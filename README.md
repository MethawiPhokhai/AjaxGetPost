Javascript call ajax Get/Post


How to call

#GET

new RequestData('@Url.Action("GetPlaceToDeliverFromJson", "PurchaseOrderPreview", null, Request.Url.Scheme)').loadData(function (data) {
  process(data);
});
                        
                        
#POST

var data = $('#addForm').serialize();
new RequestPostData('@Url.Action("UpdatePurchaseOrderMaster", "PurchaseOrderPreview", null, Request.Url.Scheme)', data).loadData();
