# webDownloader
for meany link wich download some content
for examole download attachments from yansex mails


const timer = ms => new Promise(res => setTimeout(res, ms))

async function load () {
var collection = document.getElementsByClassName("mail-ui-Button mail-ui-PseudoButton with-extras js-skip-click-message-item js-download-all-attachments");
for (let i = 0; i < collection.length; i++) {
  console.log(collection[i].href);

  collection[i].click();
 await timer(1000);
}
}



load();
