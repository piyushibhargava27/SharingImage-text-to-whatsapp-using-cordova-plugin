# SharingImage-text-to-whatsapp-using-cordova-plugin
You can share image/data to Whatsapp specific to a number or globally using Cordova plugins

Add plugin  :
  cordova plugin add cordova-plugin-x-socialsharing
  cordova prepare
  
On Button Click : 
  <button onclick="window.plugins.socialsharing.shareViaWhatsApp('Message via WhatsApp', null /* img */, null /* url */, function() {
  console.log('share ok')
  }, function(errormsg){
  alert(errormsg)})">SHARE</button>
  Sharing directly to someone
  
On a specigic phone number:
  <button onclick="window.plugins.socialsharing.shareViaWhatsAppToPhone(phone number, 'Message via WhatsApp', null /* img */, null /* url */, function() {
  console.log('share ok')
  })">SHARE</button>