<html><meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Quicksand&display=swap" rel="stylesheet"><script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><link href="https://BukaDeh.feeldream.repl.co/style.css" rel="stylesheet" type="text/css" /><script src="https://BukaDeh.feeldream.repl.co/script.js"></script>
<head>
<!-- 
This code was made by Rayya R
Blog: https://sinkronin.com
Instagram: rayyarrr
TikTok: rayyarr_
-->
</head>
<body><div id="bodyblur"><img src="https://i.postimg.cc/NMLZ6Zk5/IMG-20220207-131156-010.jpg" width="100%" height="100%"/></div>

<div id='Content'>
<div class="image"><img src="https://i.postimg.cc/dVC2C8R0/bubududu-panda-1.gif" width="130px" height="130px"/></div><!--<div id="sp1"></div>-->
<div><blockquote><p id="text"></p><p id="text2"></p><p id="akhiran" onClick="akhir();this.onclick=null;">[ Kirim Pesan &#128157; ]</p></blockquote></div></div>

<script>
  function nonFo() {document.getElementById('idfoto').style.display = "none";} function showFo() {document.getElementById('idfoto').style.display = "block";}
  function nonDiv() {document.getElementById('Content').style.display = "none";} function showDiv() {ketik();document.getElementById('Content').style.opacity = "1";document.getElementById('Content').style.margin = "0";}
  
  var i=0,text;text = ""
  var u=0,text2;text2 = ""
  
  function ketik() {if(i<text.length){document.getElementById("text").innerHTML += text.charAt(i);i++;setTimeout(ketik,100);}
    if(i==text.length){document.getElementById("text").innerHTML = text + emotnama;ketikk();}
  }
  function ketikk() {if(u<text2.length){document.getElementById("text2").innerHTML += text2.charAt(u);u++;setTimeout(ketikk,200);}
    if(u==text2.length){
    document.getElementById("text2").innerHTML = text2 + emotnama;
    document.getElementById('Content').style.animation = "kont 3s infinite";
    document.getElementById('akhiran').style = "display:block;";
    }
  }
  </script>

<script type="text/javascript">
function play() {var audio = new Audio('' + linkmp3);audio.play();}
async function akhir(){window.location = "https://api.whatsapp.com/send?phone=&text=" + pesanwhatsapp;}

            const swals = Swal.mixin({allowOutsideClick: false, cancelButtonColor: '#FF0040',});
            const swalsy = Swal.mixin({confirmButtonText: 'Iya', allowOutsideClick: false,});
            const swalst = Swal.mixin({allowOutsideClick: false, showConfirmButton: false, timer: 3000, timerProgressBar: true,});
            
            async function mulaitanya(){
            	var { isConfirmed: tanyawal } = await swals.fire({title: `Hai kamu!`, text: `Mau isi nama kamu dulu atau langsung aja?`, imageUrl: 'https://i.postimg.cc/0j2LDLxP/heart-happy.gif', imageWidth: 120, imageHeight: 120, confirmButtonText: 'Isi Nama', cancelButtonText: 'Langsung Aja', allowOutsideClick: false, showCancelButton: true,
                });if(tanyawal){mulai();} else {nama = 'Kamu';kuis();}
            }

            async function mulai(){
                var { value: nama } = await swals.fire({
                    title: 'kinsay pangalan nimo?',
                    input: 'text',
                    imageUrl: '/1.gif', imageWidth: 120, imageHeight: 120,
                    allowOutsideClick: false,
                    showCancelButton: false,
                });
                if(nama && nama.length < 11){
                	window.nama = nama;
                    pesanwhatsapp = "Aku udah liat semuanya kok><";
                    linkmp3 = 'https://Foryou.feeldream.repl.co/faudio.mp3';
                    kuis();play();
                } else {
                    await swals.fire('Ups!', 'Nama tidak boleh kosong atau lebih dari 10 karakter, ya!');
                    mulai();
                }
            }
            
            async function kuis(){
            	      await swalst.fire({
                      title: 'Hai, ' + nama + '&#129325;', 
                      imageUrl: 'https://i.postimg.cc/Nf0pkxTQ/bear-panda.gif', imageWidth: 120, imageHeight: 120,
                      });
                  	await swalst.fire({
                      title: 'hmmm crush diay tika  ' + nama + '&#128523;', 
                      imageUrl: 'https://i.postimg.cc/02wF21b1/peach-goma.gif', imageWidth: 120, imageHeight: 120,
                      });   	
                      await swalst.fire({
                      title: 'hmmm ' + nama + ' dugay na diay tika crush',
                      imageUrl: 'https://i.postimg.cc/1XScR4Vz/tkthao219-bubududu-1.gif', imageWidth: 120, imageHeight: 120,
                      });
                      await swalst.fire({
                      title: 'labyuuuu♥️',
                      imageUrl: 'https://i.postimg.cc/ydHSct1Q/gigit.gif', imageWidth: 120, imageHeight: 120,
                      });
                      await swalst.fire({
                      title: 'kapoy baya kayu buhat ani  ' + nama + ' &#128518;',
                      imageUrl: 'https://i.postimg.cc/3RXmq7fQ/mimibubu-1.gif', imageWidth: 120, imageHeight: 120,
                      });
                      text = "Hehe Pm ko sa Fb Ramil Baruiz♥️ " + nama + " Ramil :(    ";
                      emotnama = "";
                      text2 = "unta nagustohan nimo akong g buhat  <3 ";
                      showDiv();
             }
             mulai();
</script>
</body>
</html>
