task :default => [:preview]

task :preview do
  puts 'server runing'
  jekyll_pid = Process.spawn('jekyll serve --watch')
  sass_pid = Process.spawn('sass --watch _sass:public/stylesheets')

  trap('INT') do
    [jekyll_pid, sass_pid].each { |pid| Process.kill(9, pid) rescue Errno::ESRCH }
    exit 0
  end

  [jekyll_pid, sass_pid].each { |pid| Process.wait(pid) }
end

