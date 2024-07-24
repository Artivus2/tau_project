<template>
    <div>
  
     <!-- <QRCodeVue3
            value="Simple QR code"
          /> -->
  
     <QRCodeVue3
            :width="500"
            :height="500"
            value="https://836b-213-234-222-188.ngrok-free.app?company=1"
            :qrOptions="{ typeNumber: 0, mode: 'Byte', errorCorrectionLevel: 'Q' }"
            :imageOptions="{ hideBackgroundDots: true, imageSize: 0.4, margin: 0 }"
            :dotsOptions="{
            type: 'classy',
            color: '#ffffff',
            gradient: {
              type: 'linear',
              rotation: 0,
              colorStops: [
                { offset: 0, color: '#000000' },
                { offset: 1, color: '#000000' },
              ],
            },
          }"
            :backgroundOptions="{ color: '#ffffff' }"
            :cornersSquareOptions="{ type: 'dot', color: '#000000' }"
            :cornersDotOptions="{ type: undefined, color: '#000000' }"
            fileExt="png"
            :download="false"
            myclass="my-qur"
            imgclass="img-qr"
            downloadButton="my-button"
            :downloadOptions="{ name: 'vqr', extension: 'png' }"
          />
    </div>
  </template>
  
  <script>
  import QRCodeVue3 from "qrcode-vue3";
  
  export default {
    name: 'QRCodeVue3Example',
    components: {
      QRCodeVue3
    },
    
//     data: {
//     company: 'ПАО Южный Кузбасс',
//     otdel: 'Отдел управления рисками',
//     ruk: 'Ефимов А.В.',
//     subject: 'Обращение',
//     body: '-'
// }
  }
  </script>


<script>



</script>

<style>
.main-content {
display: block;
margin-top:70px;
text-align: center;
}
.main-text{

font-size: x-large;
}
</style>
