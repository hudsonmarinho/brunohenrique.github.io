---
layout: post
title: Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...
date: 2012-09-12
categories: recursos priorização pt
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed et lacus dui, a ultrices lectus. Sed vitae odio et lectus pulvinar ultrices. Mauris commodo luctus mattis. Sed eu magna eu velit lobortis luctus non facilisis dui. Vivamus consectetur adipiscing odio, sit amet commodo dui posuere porta. Aenean porta velit quis lorem egestas quis feugiat augue vehicula. Etiam purus neque, imperdiet eu blandit id, venenatis eget neque. Nullam lobortis nibh nec felis commodo euismod quis congue tortor. Praesent dapibus malesuada convallis.

Nunc ac risus eu lacus gravida facilisis. Proin mattis tellus sit amet leo iaculis at eleifend urna pulvinar. Fusce ullamcorper pharetra luctus. Ut massa lorem, lacinia elementum accumsan sed, lobortis sit amet turpis. Sed tellus massa, ullamcorper eu convallis quis, gravida a ipsum. Nulla eget rhoncus velit. Integer et tortor nunc. Phasellus nisl elit, suscipit sed egestas elementum, interdum sed diam.

Donec commodo gravida odio, quis dapibus risus porta rutrum. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vivamus erat urna, hendrerit nec dignissim eu, condimentum vel est. Aenean mattis, est eget eleifend suscipit, enim est tempor nisi, nec gravida lacus felis non nibh. Curabitur aliquam dictum sapien non ultricies. Etiam tincidunt blandit velit quis eleifend. Integer consectetur nisl non est lobortis et malesuada arcu volutpat. Maecenas faucibus odio eu sapien eleifend a varius mauris dapibus. Nullam ac ornare ante. Aliquam quis magna sed erat sodales commodo. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Aenean consectetur, libero a semper tristique, eros metus varius ipsum, ut volutpat odio nulla id lacus. Duis a quam sit amet lectus volutpat commodo et quis augue. Morbi vitae leo vel nulla imperdiet feugiat nec hendrerit tellus.

Integer vitae lacus et libero tincidunt lacinia nec sit amet mi. Vestibulum ultrices turpis ut enim vestibulum congue. Mauris sapien elit, accumsan et sagittis laoreet, eleifend nec leo. Maecenas a elit nibh. Maecenas eget velit quis augue elementum sagittis sit amet ut enim. Aliquam erat nisi, pulvinar in tincidunt eu, hendrerit et tellus. Pellentesque ante ante, convallis sed ultricies nec, porttitor et eros. Pellentesque sagittis viverra mi non vehicula. Duis ut sapien nunc, at venenatis nulla. Ut tempor malesuada mi nec laoreet. Maecenas ultrices, dui eleifend consequat pellentesque, lorem ipsum tristique libero, eget auctor eros nisi et velit. Phasellus sit amet scelerisque tellus.

Nullam semper lacus enim. Fusce molestie ipsum semper dui vulputate vitae vulputate diam molestie. Vivamus pulvinar sem non turpis commodo a fermentum orci posuere. Nullam quis leo venenatis velit varius mattis non sed nulla. Cras pulvinar semper lorem eget scelerisque. Aliquam tempor tempor risus, id bibendum orci blandit vel. Nulla facilisi. Phasellus vitae pharetra magna. Integer in rutrum tellus. Donec molestie, felis sed auctor fringilla, nisl sapien laoreet purus, eget placerat diam dui quis nunc. Nulla facilisi. Vivamus dictum nulla ac neque molestie eu commodo lacus convallis.

<!-- more start -->

**Limitações são libertadoras.**
{% highlight ruby linenos %}
## PayRoll gem

# lib/pay_roll.rb
module PayRoll
  class << self
    attr_accessor :employee_directory
      def config
        yield self
      end
    end
  end
end

# lib/pay_roll/services/pay_day_service.rb
class PayRoll::PayDayService
  def initialize(date=Date.now)
    @date = date

    @employees = PayRoll.employee_directory.active
    @employees.each { |e| e.extend(Payable) }
  end
{% endhighlight %}

{% highlight javascript linenos %}
$(document).ready(function() {
    $("#link_search").click(function() {
        var urlSearch = $(this).val()
        $.ajax({
            type: "POST",
            url: "/search",
            data: {urlSearch: urlSearch},
            success: function(data) {
                alert(data);
            },
            error: function(data) {
                alert('erro');
            }
        });
    });
});
{% endhighlight %}

Suspendisse mattis, dui quis fringilla commodo, diam tortor rhoncus dolor, vel pharetra enim libero a velit. Ut vel erat diam, ut dignissim justo. Nullam imperdiet aliquam augue, et tristique ligula tempor sagittis. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nunc condimentum rutrum elit at mollis. Maecenas sit amet elementum enim. Quisque mollis, diam in ultricies molestie, tellus libero condimentum purus, non sollicitudin libero justo ac dolor. Etiam ante lectus, cursus vitae porta et, aliquam id lectus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce volutpat suscipit enim, sed hendrerit diam posuere vel. Nulla eget enim in est faucibus porttitor. Cras venenatis commodo semper. Donec sed arcu dui. Curabitur eget sapien odio. Nam et lacus libero.

Mauris vel accumsan orci. Aliquam mauris nulla, convallis vel tincidunt eget, vulputate in risus. Sed risus metus, molestie ullamcorper suscipit sit amet, molestie quis metus. Praesent nibh nibh, condimentum at luctus quis, interdum et nisl. Vestibulum tincidunt faucibus porttitor. Phasellus eu massa eget turpis consectetur eleifend. Maecenas vel purus ligula, et congue est. Duis mauris lorem, venenatis et fringilla sit amet, ullamcorper nec enim. Duis nec orci mauris. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla facilisi. Sed ante mi, pellentesque non rutrum ut, placerat eu metus. Pellentesque pretium imperdiet turpis, nec suscipit dui pharetra luctus. Cras risus leo, molestie ut faucibus a, eleifend et leo. Sed ultricies arcu vitae mi ornare blandit.

Sed pharetra justo lobortis turpis dictum ac pretium nisi consectetur. Nulla justo nulla, lacinia vitae feugiat ut, accumsan non diam. Quisque arcu tellus, aliquet venenatis scelerisque a, feugiat at magna. Pellentesque ac odio sed enim ultricies viverra. Ut sodales, nisi eget laoreet scelerisque, eros orci faucibus nisl, at aliquet nunc urna et elit. Mauris malesuada convallis quam, aliquet interdum massa iaculis quis. Maecenas id justo risus, eu semper erat. Morbi arcu eros, consequat eu cursus quis, porttitor sit amet quam. Donec tellus eros, pharetra vitae fringilla ac, tincidunt id risus.

<!-- more end -->
