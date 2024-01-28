const cold = document.createElement("h3");
cold.id = "shfhhswu";
document.body.appendChild(cold);

Object.assign(cold.style, {
  backgroundColor: "black",
  width: '0',
  color: "white",
  fontSize: "21px",
  zIndex: "110",
  position: "absolute",
  padding: "10px",
  fontFamily: "revert",
  fontWeight: "normal",
  left: '0',
  top: '0',
  
  
});


const contentLineas= document.getElementById("gameScreen");
const canvas=document.createElement("canvas");
canvas.style.width = '100%';
canvas.style.height = '100%';
contentLineas.appendChild(canvas); 
const ctx = canvas.getContext('2d');
const ctx2 = canvas.getContext('2d');

canvas.width = 809;
canvas.height = 607;

const contenedor=document.getElementById("gameui"); 
const contenedorHijo = document.createElement("div");
contenedorHijo.id = "contentHijo";


contenedor.appendChild(contenedorHijo);

Object.assign(contenedorHijo.style, {
  backgroundColor: "rgba(0, 0, 0, 0.3)",
  width: '25%',
  height: '40px',
  zIndex: "110",
  position: "absolute",
  padding: "10px",
  display: 'flex',
  justifyContent: 'center',
  alignItems: 'center',
  borderRadius: '10px',
  left: '40%',
  top:'-80%', 
});

const inputs = document.createElement('input');
    inputs.type = 'range';
    inputs.id = 'miTrackbar';
    inputs.min = '-50';
    inputs.max = '50';
    inputs.value = '0';
    inputs.step = '1';



  let styleSheet = document.styleSheets[0];
  styleSheet.insertRule('#miTrackbar::-webkit-slider-runnable-track { background-color:white; border-radius: 8px', 0);

  const decrementarBtn = document.createElement('button');
  decrementarBtn.textContent = '-';
  decrementarBtn.id = 'decrementar';


  const incrementarBtn = document.createElement('button');
  incrementarBtn.textContent = '+';
  incrementarBtn.id = 'incrementar';

  Object.assign(inputs.style,{
  zIndex: "200",
  cursor: 'pointer',
  });

  Object.assign(decrementarBtn.style,{
  zIndex: "200",
  cursor: 'pointer',
  padding: '4px',
   fontSize: "22px",
   width: '30px',
  });

  Object.assign(incrementarBtn.style,{
  zIndex: "200",
  cursor: 'pointer',
  padding: '4px',
  fontSize: "22px",
   width: '30px',
  });


  contenedorHijo.appendChild(decrementarBtn);
  contenedorHijo.appendChild(inputs);
  contenedorHijo.appendChild(incrementarBtn);

  const valorActual = document.createElement('p');
  Object.assign(valorActual.style,{
  zIndex: "220",
  cursor: 'pointer',
  padding: '4px',
  fontSize: '15px',
  color: 'black',
  width: '20%',
  backgroundColor: 'white',
  textAlign: 'center',
  borderRadius: '4px',
  });

  const divCentrar = document.createElement('div');
    Object.assign(divCentrar.style,{
      zIndex: "200",
      cursor: 'pointer',
      width: '100%',
      height:'30%',
      position: 'absolute',
      display: 'flex',
      justifyContent: 'center',
      alignItems: 'center',
      top: '0',     
  });

  contenedorHijo.appendChild(divCentrar);
  divCentrar.appendChild(valorActual);



    function actualizarValor() {
      valorActual.textContent = (parseInt(inputs.value)/4).toFixed(2);
    }

 inputs.addEventListener('input', actualizarValor);

 incrementarBtn.addEventListener('click', function() {
      inputs.value = parseInt(inputs.value, 10) + 1;
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });

  incrementarBtn.addEventListener('touchstart', function() {
      inputs.value = parseInt(inputs.value, 10) + 1;
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });

    decrementarBtn.addEventListener('click', function() {
      inputs.value = parseInt(inputs.value, 10) - 1;
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });

    decrementarBtn.addEventListener('touchstart', function() {
      inputs.value = parseInt(inputs.value, 10) - 1;
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });


    valorActual.addEventListener('click', function() {
      inputs.value = parseInt(0);
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });

    valorActual.addEventListener('touchstart', function() {
      inputs.value = parseInt(0);
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
    });


actualizarValor();

function crearlineas(color, grosor, x1, y1, x2, y2) {
    
    ctx.strokeStyle = color;
    ctx.lineWidth = grosor;
    ctx.beginPath();
    ctx.moveTo(x1, y1);
    ctx.lineTo(x2, y2);
    ctx.stroke();
}



const barraPoder = document.getElementById('powerMarkArea');
const rallita = document.createElement('div');
    Object.assign(rallita.style,{
      zIndex: "200",
      width: '2px',
      height:'66%',
      opacity: '1',
      position: 'absolute',
      backgroundColor: 'blue',
      top: '0',
      left:'0',     
  });

const rallita2 = document.createElement('div');
    Object.assign(rallita2.style,{
      zIndex: "200",
      width: '2px',
      height:'66%',
      opacity: '1',
      position: 'absolute',
      backgroundColor: 'black',
      top: '0',
      left:'0',     
  });

const rallita3 = document.createElement('div');
    Object.assign(rallita3.style,{
      zIndex: "200",
      width: '2px',
      height:'66%',
      opacity: '1',
      position: 'absolute',
      backgroundColor: 'red',
      top: '0',
      left:'0',     
  });

const rallita4 = document.createElement('div');
    Object.assign(rallita4.style,{
      zIndex: "200",
      width: '2px',
      height:'66%',
      opacity: '1',
      position: 'absolute',
      backgroundColor: 'white',
      top: '0',
      left:'0',     
  });




barraPoder.appendChild(rallita);
barraPoder.appendChild(rallita2);
barraPoder.appendChild(rallita3);
barraPoder.appendChild(rallita4);


//crear nombres::::
const p1 = document.createElement('h5');
    Object.assign(p1.style,{
      zIndex: "200",
      fontSize: '8px',
      opacity: '1',
      position: 'absolute',
      top: '1px',
      left:'0',     
  });

const p2 = document.createElement('h5');
    Object.assign(p2.style,{
      zIndex: "200",
      fontSize: '8px',
      opacity: '1',
      position: 'absolute',
      top: '4px',
      left:'0',     
  });

const p3 = document.createElement('h5');
    Object.assign(p3.style,{
      zIndex: "200",
      fontSize: '8px',
      opacity: '1',
      position: 'absolute',
      top: '8px',
      left:'0',     
  });

const p4 = document.createElement('h5');
    Object.assign(p4.style,{
      zIndex: "200",
      fontSize: '8px',
      opacity: '1',
      position: 'absolute',
      top: '13px',
      left:'0',     
  });


barraPoder.appendChild(p1);
barraPoder.appendChild(p2);
barraPoder.appendChild(p3);
barraPoder.appendChild(p4);

//autoshot---------------------------------

const contentBotones=document.createElement('div');
Object.assign(contentBotones.style, {
  zIndex: "107",
  width: '150px',
  alignItems: 'center',
  justifyContent: 'center',
  height: '40px',
  gap:'4px',
  display: 'flex',
  position: "absolute",
  right: '0',
  top: '0',
  
});

const botonShot=document.createElement('button');
botonShot.textContent='1';
Object.assign(botonShot.style, {
  backgroundColor: "blue",
  fontSize: '12px',
  color: "white",
  cursor: 'pointer',
  display: 'none',
  zIndex: "110",
  padding: "10px",
  flex: '1',
  fontFamily: "revert",
  fontWeight: "normal",

  
});

const botonShot2=document.createElement('button');
botonShot2.textContent='2';
Object.assign(botonShot2.style, {
  backgroundColor: "black",
  color: "white",
  fontSize: '12px',
  cursor: 'pointer',
  flex: '1',
  zIndex: "110",
  display: 'none',
  padding: "10px",
  fontFamily: "revert",
  fontWeight: "normal",

  
});

const botonShot3=document.createElement('button');
botonShot3.textContent='3';
Object.assign(botonShot3.style, {
  backgroundColor: "red",
  color: "white",
  fontSize: '12px',
  flex: '1',
  cursor: 'pointer',
  display: 'none',
  zIndex: "110",
  padding: "10px",
  fontFamily: "revert",
  fontWeight: "normal",

  
});

const botonShot4=document.createElement('button');
botonShot4.textContent='4';
Object.assign(botonShot4.style, {
  backgroundColor: "white",
  fontSize: '12px',
  color: "black",
  zIndex: "110",
  cursor: 'pointer',
  display: 'none',
  padding: "10px",
  flex: '1',
  fontFamily: "revert",
  fontWeight: "normal",

  
});

contenedor.appendChild(contentBotones);

contentBotones.appendChild(botonShot);
contentBotones.appendChild(botonShot2);
contentBotones.appendChild(botonShot3);
contentBotones.appendChild(botonShot4);



botonShot.addEventListener('click', function() {
  if(dragon2d.players[indice].hp!=0){
     if(typeof ct==='undefined'){
      ct=29384;
      }  

   dragon2d.players[indice].Shoot(shot,ct,dragon2d.players[indice].selected_shot,dragon2d.stat);
    $("#powerBar").css("width", poderio);
  }
});


botonShot2.addEventListener('click', function() {
  if(dragon2d.players[indice].hp!=0){
     if(typeof ct==='undefined'){
      ct=29384;
      }  
   dragon2d.players[indice].Shoot(shot2,ct,dragon2d.players[indice].selected_shot,dragon2d.stat);
    $("#powerBar").css("width", poderio2);
  }
});


botonShot3.addEventListener('click', function() {
     if(typeof ct==='undefined'){
      ct=29384;
      }  
  if(dragon2d.players[indice].hp!=0){
   dragon2d.players[indice].Shoot(shot3,ct,dragon2d.players[indice].selected_shot,dragon2d.stat);
    $("#powerBar").css("width", poderio3);
  }
});


botonShot4.addEventListener('click', function() {
     if(typeof ct==='undefined'){
      ct=29384;
      }  
  if(dragon2d.players[indice].hp!=0){
   dragon2d.players[indice].Shoot(shot4,ct,dragon2d.players[indice].selected_shot,dragon2d.stat);
    $("#powerBar").css("width", poderio4);
  }
});


//-----------------------------------------



let distanciax = 0;
let distanciay = 0;

let distanciax2 = 0;
let distanciay2 = 0;

let distanciax3 = 0;
let distanciay3 = 0;

let distanciax4 = 0;
let distanciay4 = 0;
let calibrador = 0.004332712;

const capturarId = () => {
  try {
    const myId = dragon2d.my_user_id;
    for (let i = 0; i < 8; i++) {
      try {
        if (dragon2d.players[i].id === myId) {
          let team = dragon2d.players[i].team;
          let teamContrario=separarEquipo(team);
          extraerDatos(i,teamContrario);
          break;
        }
      } catch (error) {}
    }
  } catch (error) {}
  setTimeout(capturarId, 1);
};
capturarId();

//equipo contrario
const separarEquipo=(equipacho)=>{
  let equipo=[];
  for(let j=0;j<dragon2d.players.length;j++){
    if(dragon2d.players[j].team!=equipacho){
      equipo.push(j);
    }
  }

 return equipo
}




const nombreJugador=(s,nombre)=>{
   let nombreJug=(dragon2d.players[+s].name).split(' ');
   nombre.textContent=`${nombreJug[0]}`;
}




let indice=0;
const extraerDatos =(x,teamCo)=> {

  indice=x;
  const ccc = parseFloat(pantalla.cameraScale);  
  const ldb = dragon2d.players[x].look;
  const mb = (dragon2d.players[x].mobile);
  //const ccc = cc.toString().substring(0, 4);
  //const curPower=dragon2d.curUIPower;
  const jugadores=dragon2d.players.length;
 




  if(typeof dragon2d.dragon2d==='undefined'){
      inputs.value = parseInt(0);
      calibrador=parseFloat((inputs.value))*0.000047 + 0.004332712
      actualizarValor();
     
  }





 switch (jugadores) {

   case 2:
    if(dragon2d.players[+teamCo[0]].hp!=0){
        distanciax = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot.style.display= 'block';
       }else{
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';

       }

       if((ldb==0 && Math.sign(distanciax)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax)==1 && (mb!=2 && mb!=11))){
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax)==1 && (mb==2 || mb==11))){
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';
       }


        nombreJugador(teamCo[0],p1);

         distanciax2 = 0;
         distanciay2 = 0;

         distanciax3 = 0;
         distanciay3 = 0;

         distanciax4 = 0;
         distanciay4 = 0;

        botonShot2.style.display= 'none';
        botonShot3.style.display= 'none';
        botonShot4.style.display= 'none';

        if(dragon2d.players[x].hp==0){
          distanciax=0;
          distanciay=0;

          distanciax2 = 0;
          distanciay2 = 0;

          distanciax3 = 0;
          distanciay3 = 0;

          distanciax4 = 0;
          distanciay4 = 0;

          botonShot.style.display= 'none';
          botonShot2.style.display= 'none';
          botonShot3.style.display= 'none';
          botonShot4.style.display= 'none';

         }
    
   break;

   case 4:

      if(dragon2d.players[+teamCo[0]].hp!=0){
        distanciax = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot.style.display= 'block';
      }else{
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';    
      }

       if((ldb==0 && Math.sign(distanciax)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax)==1 && (mb!=2 && mb!=11))){
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax)==1 && (mb==2 || mb==11))){
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';
       }


      if(dragon2d.players[+teamCo[1]].hp!=0){
        distanciax2 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay2 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot2.style.display= 'block';
        }else{
        distanciax2=0;
        distanciay2=0; 
        botonShot2.style.display= 'none'; 
        }

       if((ldb==0 && Math.sign(distanciax2)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax2)==1 && (mb!=2 && mb!=11))){
        distanciax2=0;
        distanciay2=0;
         botonShot2.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax2)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax2)==1 && (mb==2 || mb==11))){
        distanciax2=0;
        distanciay2=0;
        botonShot2.style.display= 'none';
       }

         nombreJugador(teamCo[0],p1);
         nombreJugador(teamCo[1],p2);

         distanciax3 = 0;
         distanciay3 = 0;

         distanciax4 = 0;
         distanciay4 = 0;

         botonShot3.style.display= 'none';
         botonShot4.style.display= 'none';

        if(dragon2d.players[x].hp==0){
          distanciax=0;
          distanciay=0;

          distanciax2 = 0;
          distanciay2 = 0;

          distanciax3 = 0;
          distanciay3 = 0;

          distanciax4 = 0;
          distanciay4 = 0;

          botonShot.style.display= 'none';
          botonShot2.style.display= 'none';
          botonShot3.style.display= 'none';
          botonShot4.style.display= 'none';
         }
    

   break;

 case 6:

      if(dragon2d.players[+teamCo[0]].hp!=0){
        distanciax = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.ty) / ccc;
         botonShot.style.display= 'block';
        }else{
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';   
        }

       if((ldb==0 && Math.sign(distanciax)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax)==1 && (mb!=2 && mb!=11))){
        distanciax=0;
        distanciay=0;
         botonShot.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax)==1 && (mb==2 || mb==11))){
        distanciax=0;
        distanciay=0;
         botonShot.style.display= 'none';
       }




      if(dragon2d.players[+teamCo[1]].hp!=0){
        distanciax2 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay2 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot2.style.display= 'block';
        }else{
        distanciax2=0;
        distanciay2=0;
        botonShot2.style.display= 'none';
        }

       if((ldb==0 && Math.sign(distanciax2)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax2)==1 && (mb!=2 && mb!=11))){
        distanciax2=0;
        distanciay2=0;
         botonShot2.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax2)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax2)==1 && (mb==2 || mb==11))){
        distanciax2=0;
        distanciay2=0;
         botonShot2.style.display= 'none';
       }



      if(dragon2d.players[+teamCo[2]].hp!=0){
        distanciax3 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[2]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay3 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[2]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot3.style.display= 'block';
        }else{
        distanciax3=0;
        distanciay3=0;
        botonShot3.style.display= 'none';
        }

       if((ldb==0 && Math.sign(distanciax3)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax3)==1 && (mb!=2 && mb!=11))){
        distanciax3=0;
        distanciay3=0;
         botonShot3.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax3)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax3)==1 && (mb==2 || mb==11))){
        distanciax3=0;
        distanciay3=0;
        botonShot3.style.display= 'none';
       }


        nombreJugador(teamCo[0],p1);
        nombreJugador(teamCo[1],p2);
        nombreJugador(teamCo[2],p3);

         distanciax4 = 0;
         distanciay4 = 0;
         botonShot4.style.display= 'none';

        if(dragon2d.players[x].hp==0){
          distanciax=0;
          distanciay=0;

          distanciax2 = 0;
          distanciay2 = 0;

          distanciax3 = 0;
          distanciay3 = 0;

          distanciax4 = 0;
          distanciay4 = 0;

          botonShot.style.display= 'none';
          botonShot2.style.display= 'none';
          botonShot3.style.display= 'none';
          botonShot4.style.display= 'none';
         }
    

   break;
 case 8:
      if(dragon2d.players[+teamCo[0]].hp!=0){
        distanciax = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[0]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot.style.display= 'block';
        }else{
          distanciax=0;
          distanciay=0;
          botonShot.style.display= 'none';

        }

       if((ldb==0 && Math.sign(distanciax)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax)==1 && (mb!=2 && mb!=11))){
        distanciax=0;
        distanciay=0;
        botonShot.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax)==1 && (mb==2 || mb==11))){
        distanciax=0;
        distanciay=0;
         botonShot.style.display= 'none';
       }


      if(dragon2d.players[+teamCo[1]].hp!=0){
        distanciax2 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay2 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[1]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot2.style.display= 'block';
        }else{
          distanciax2=0;
          distanciay2=0;
          botonShot2.style.display= 'none';
        }

       if((ldb==0 && Math.sign(distanciax2)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax2)==1 && (mb!=2 && mb!=11))){
        distanciax2=0;
        distanciay2=0;
         botonShot2.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax2)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax2)==1 && (mb==2 || mb==11))){
        distanciax2=0;
        distanciay2=0;
         botonShot2.style.display= 'none';
       }


      if(dragon2d.players[+teamCo[2]].hp!=0){
        distanciax3 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[2]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay3 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[2]].player_sprite.player_info.worldTransform.ty) / ccc;
         botonShot3.style.display= 'block';
       }else{
        distanciax3 =0;
        distanciay3=0;
         botonShot3.style.display= 'none';
       }

       if((ldb==0 && Math.sign(distanciax3)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax3)==1 && (mb!=2 && mb!=11))){
        distanciax3=0;
        distanciay3=0;
         botonShot3.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax3)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax3)==1 && (mb==2 || mb==11))){
        distanciax3=0;
        distanciay3=0;
         botonShot3.style.display= 'none';
       }


      if(dragon2d.players[+teamCo[3]].hp!=0){
        distanciax4 = (dragon2d.players[x].player_sprite.angle.worldTransform.tx - dragon2d.players[+teamCo[3]].player_sprite.player_info.worldTransform.tx) / ccc;
        distanciay4 = (dragon2d.players[x].player_sprite.angle.worldTransform.ty - dragon2d.players[+teamCo[3]].player_sprite.player_info.worldTransform.ty) / ccc;
        botonShot4.style.display= 'block';
      }else{
        distanciax4=0;
        distanciay4=0;
        botonShot4.style.display= 'none';
      }

       if((ldb==0 && Math.sign(distanciax4)==-1 && (mb!=2 && mb!=11)) || (ldb==1 && Math.sign(distanciax4)==1 && (mb!=2 && mb!=11))){
        distanciax4=0;
        distanciay4=0;
         botonShot4.style.display= 'none';
       }


       if((ldb==1 && Math.sign(distanciax4)==-1 && (mb==2 || mb==11)) || (ldb==0 && Math.sign(distanciax4)==1 && (mb==2 || mb==11))){
        distanciax4=0;
        distanciay4=0;
         botonShot4.style.display= 'none';
       }

        nombreJugador(teamCo[0],p1);
        nombreJugador(teamCo[1],p2);
        nombreJugador(teamCo[2],p3);
        nombreJugador(teamCo[3],p4);

        if(dragon2d.players[x].hp==0){
          distanciax=0;
          distanciay=0;

          distanciax2 = 0;
          distanciay2 = 0;

          distanciax3 = 0;
          distanciay3 = 0;

          distanciax4 = 0;
          distanciay4 = 0;

          botonShot.style.display= 'none';
          botonShot2.style.display= 'none';
          botonShot3.style.display= 'none';
          botonShot4.style.display= 'none';
         }
    

   break;



 }



  
  const tf = document.getElementById("Dragon2D").style.transform;
  const cn = tf.slice(22, -5) === '' ? 0 : parseInt(tf.slice(22, -5));

  const ld = ldb ? -1 : 1;
  const an = dragon2d.players[x].ang + dragon2d.players[x].body * ld;
  const dx = dragon2d.players[x].player_sprite.aimCircle.worldTransform.tx + cn;
  const dy = dragon2d.players[x].player_sprite.aimCircle.worldTransform.ty;
  const ax = wina;
  const ay = winb;
  const pantallaX = pantalla.renderer.gl.drawingBufferWidth/ccc;
  const pantallaY = pantalla.renderer.gl.drawingBufferHeight/ccc;
  const barraPoderX =parseInt(pantalla.renderer.projection.x);
  
  let masa = 0.023430;
  let gravedad = 0;
  let fuerzaViento = ax;
  let lado = ldb;
  let anguloCarro = an;
  let anguloViento = ay;

canvas.width = pantallaX;
canvas.height = pantallaY;


    switch ((mb)) {
  case 0:
    //armor
       masa = 0.257208;
       gravedad = 380;
     //cold.innerHTML = `${mb} armor`;
     break;

  case 1:
    //ice
       masa = 0.3033;
       gravedad = 327;
     //cold.innerHTML = `${mb} ice`;
    break;
  case 2:
    //aduka
      masa = 0.2855;
      gravedad = 334;
      anguloCarro = 180-an;
     //cold.innerHTML = `${mb} aduka ${anguloCarro}`;
     break;

 case 3:
   //cold.innerHTML = `${an} Lightning`;
      masa = 0.27545;
      gravedad = 333;
    break;

 case 4:
   //cold.innerHTML = `${mb} big`;
      masa = 0.21599;
      gravedad = 466;
    break;

 case 5:
   //cold.innerHTML = `${mb} jd`;
      masa = 0.3033;
      gravedad = 327;
    break;

 case 6:
   //cold.innerHTML = `${mb} asate`;
      masa = 0.25561;
      gravedad = 389;
    break;
  case 8:
   //cold.innerHTML = `${mb} caballo`;
      masa = 0.25561;
      gravedad = 389;
    break;

  case 9:
   //cold.innerHTML = `${mb} fox`;
      masa = 0.24545;
      gravedad = 320;
    break;

  case 10:
   //cold.innerHTML = `${mb} barnie`;
      masa = 0.2235;
      gravedad = 495;
    break;    

 case 11:
   anguloCarro = 180-an;
   //cold.innerHTML = `${mb} nak an${anguloCarro}`;
      masa = 0.20985;
      gravedad = 438;
    break;

 case 12:
   //cold.innerHTML = `${mb} trico an${an}`;
      masa = 0.23554;
      gravedad = 428;
    break;

 case 13:
   //cold.innerHTML = `${mb} mago an${an}`;
      masa = 0.24845;
      gravedad = 364;
    break;

 case 14:
   //cold.innerHTML = `${mb} turtle an${an}`;
      masa = 0.254;
      gravedad = 380;
    break;

 case 15:
   //cold.innerHTML = `${mb} boomer an${an}`;
      masa = 0.14697;
      gravedad = 324;
    break;

 case 16:
   //cold.innerHTML = `${mb} electrico an${an}`;
      masa = 0.25855;
      gravedad = 379;
    break;

 case 17:
   //cold.innerHTML = `${mb} grub an${an}`;
      masa = 0.3023;
      gravedad = 327;
    break;

 case 18:
   //cold.innerHTML = `${mb} dragon an${an}`;
      masa = 0.2235;
      gravedad = 495;
    break;

 case 19:
   //cold.innerHTML = `${mb} roan angulo ${an}`;
      masa = 0.23754;
      gravedad = 412;
    break;

 case 20:
   //cold.innerHTML = `${mb} randomixer angulo ${an}`;
      masa = 0.26445;
      gravedad = 333;
    break;

 case 21:
   //cold.innerHTML = `${mb} sapo an${an}`;
      masa = 0.3286545;
      gravedad = 284;
    break;

 case 22:
   //cold.innerHTML = `${mb} calsidon an${an}`;
      masa = 0.2825;
      gravedad = 362;
    break;
};



  if(mb==2 || mb==11){
    if(lado==1){
      if(ay>=0 && ay<=180){
      anguloViento=(180-ay);
      }else if(ay>180 && ay<=360){
      anguloViento=360 + (180-ay);
      }
    }
  }else{
    if(lado==0){
      if(ay>=0 && ay<=180){
      anguloViento=(180-ay);
      }else if(ay>180 && ay<=360){
      anguloViento=360 + (180-ay);
      }
    }
  }


  let anguloRadianes = anguloCarro * (Math.PI / 180);
  let cosenoAngulo = Math.cos(anguloRadianes);
  let senoAngulo = Math.sin(anguloRadianes);
  let windAnguloRadianes = anguloViento * (Math.PI / 180);
  let senoWind = Math.sin(windAnguloRadianes);
  let cosenoWind = Math.cos(windAnguloRadianes);
  let xfuerza = cosenoWind * fuerzaViento;
  let yfuerza = senoWind * fuerzaViento;
  let xaceleracion = xfuerza / masa;

  let yaceleracion = (gravedad - yfuerza / masa);
  let tangente = Math.tan(anguloCarro * Math.PI / 180);


  let distX = (Math.abs(distanciax / pantallaX * 800))/ccc;
  let distaY = (distanciay / pantallaY * 600)/ccc;

  let distX2 = (Math.abs(distanciax2 / pantallaX * 800))/ccc;
  let distaY2 = (distanciay2 / pantallaY * 600)/ccc;

  let distX3 = (Math.abs(distanciax3 / pantallaX * 800))/ccc;
  let distaY3 = (distanciay3 / pantallaY * 600)/ccc;

  let distX4 = (Math.abs(distanciax4 / pantallaX * 800))/ccc;
  let distaY4 = (distanciay4 / pantallaY * 600)/ccc;

//autocalibracion aca 
  let tiempo = Math.sqrt((2 * distX * tangente - 2 * distaY) / (yaceleracion + tangente * xaceleracion));
  let tiempo2 = Math.sqrt((2 * distX2 * tangente - 2 * distaY2) / (yaceleracion + tangente * xaceleracion));
  let tiempo3 = Math.sqrt((2 * distX3 * tangente - 2 * distaY3) / (yaceleracion + tangente * xaceleracion));
  let tiempo4 = Math.sqrt((2 * distX4 * tangente - 2 * distaY4) / (yaceleracion + tangente * xaceleracion));

  let xvelocidad = (distX - (xaceleracion * 0.5 * Math.pow(tiempo, 2))) / tiempo;
  let xvelocidad2 = (distX2 - (xaceleracion * 0.5 * Math.pow(tiempo2, 2))) / tiempo2;
  let xvelocidad3 = (distX3 - (xaceleracion * 0.5 * Math.pow(tiempo3, 2))) / tiempo3;
  let xvelocidad4 = (distX4 - (xaceleracion * 0.5 * Math.pow(tiempo4, 2))) / tiempo4;

  let yvelocidad = (distaY + (yaceleracion * Math.pow(tiempo, 2) * 0.5)) / tiempo;
  let yvelocidad2 = (distaY2 + (yaceleracion * Math.pow(tiempo2, 2) * 0.5)) / tiempo2;
  let yvelocidad3 = (distaY3 + (yaceleracion * Math.pow(tiempo3, 2) * 0.5)) / tiempo3;
  let yvelocidad4 = (distaY4 + (yaceleracion * Math.pow(tiempo4, 2) * 0.5)) / tiempo4;


  let velocidadIni = Math.sqrt(Math.pow(xvelocidad, 2) + Math.pow(yvelocidad, 2));
  let velocidadIni2 = Math.sqrt(Math.pow(xvelocidad2, 2) + Math.pow(yvelocidad2, 2));
  let velocidadIni3 = Math.sqrt(Math.pow(xvelocidad3, 2) + Math.pow(yvelocidad3, 2));
  let velocidadIni4 = Math.sqrt(Math.pow(xvelocidad4, 2) + Math.pow(yvelocidad4, 2));

   ctx.clearRect(0, 0, pantallaX, pantallaY); 
   ctx2.clearRect(0, 0, pantallaX, pantallaY);

  if(jugadores==2){

    formandoLineas(ldb,xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'blue',dx,dy,mb);
    //cold.innerHTML = `${mb}|${ldb}|${Math.round(an)}|${parseInt(distanciax)}|${Math.round(distanciay)}|${ax}|${ay}|${Math.round(dx)}|${Math.round(dy)}|${ccc}`;
    if(mb==0 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'blue');
      }else if(mb==15 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'blue');
      }else if(mb==14 && dragon2d.players[x].selected_shot==1){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'blue');
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'blue');
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'blue');
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'blue');
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'blue');
      }else if(mb==12 && dragon2d.players[x].selected_shot==1){
         //cold.innerHTML = `trico2`;

            if(ldb==0){                                                                                           //2.160
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'blue');
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'blue'); //3.338 parseFloat(numericaUp.value)
            }else if(ldb==1){
              //>>> 1 
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'blue');
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'blue');//perfecto
            }

      }else if(mb==17 && dragon2d.players[x].selected_shot==1){
        //cold.innerHTML = `grub2`;

            if(ldb==0){                                                                                           
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'blue');
              
            }else if(ldb==1){
              //>>> 1
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'blue');
              
            }

      }


  }else if(jugadores==4){

    formandoLineas(ldb,xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'blue',dx,dy,mb);
    formandoLineas(ldb,xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'black',dx,dy,mb);

      if(mb==0 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'black');
      }else if(mb==15 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'black');
      }else if(mb==14 && dragon2d.players[x].selected_shot==1){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'black');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'black');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'black');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'black');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'black');
      }else if(mb==12 && dragon2d.players[x].selected_shot==1){
        //cold.innerHTML = `trico4`;

            if(ldb==0){                                                                                        
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'black');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'black'); 
            }else if(ldb==1){
              //>>> 1 
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'black');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'black');
            }

      }else if(mb==17 && dragon2d.players[x].selected_shot==1){
        //cold.innerHTML = `grub4`;

            if(ldb==0){                                                                                           
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'black');

            }else if(ldb==1){
              //>>> 1
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'black');
              
            }

      }



  }else if(jugadores==6){

    formandoLineas(ldb,xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'blue',dx,dy,mb);

    formandoLineas(ldb,xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'black',dx,dy,mb);

    formandoLineas(ldb,xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'red',dx,dy,mb);

      if(mb==0 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'red');
      }else if(mb==15 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'red');
      }else if(mb==14 && dragon2d.players[x].selected_shot==1){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'red');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'red');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'red');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'red');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'red');
      }else if(mb==12 && dragon2d.players[x].selected_shot==1){
          //cold.innerHTML = `trico6`;
            if(ldb==0){                                                                                        
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'red');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'red'); 
            }else if(ldb==1){
              //>>> 1 
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'red');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'red');
            }

      }else if(mb==17 && dragon2d.players[x].selected_shot==1){

            //cold.innerHTML = `grub6`;
            if(ldb==0){                                                                                           
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'red');

            }else if(ldb==1){
              //>>> 1
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'red');
              
            }

      }



  }else if(jugadores==8){

    formandoLineas(ldb,xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'blue',dx,dy,mb);

    formandoLineas(ldb,xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'black',dx,dy,mb);

    formandoLineas(ldb,xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'red',dx,dy,mb);

    formandoLineas(ldb,xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,'white',dx,dy,mb);

      if(mb==0 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.8863,'white');
      }else if(mb==15 && dragon2d.players[x].selected_shot==2){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.4563,'white');
      }else if(mb==14 && dragon2d.players[x].selected_shot==1){
        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.567,'white');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,0.9,'white');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.16,'white');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.45,'white');

        crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'blue');
        crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'black');
        crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'red');
        crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.84,'white');
      }else if(mb==12 && dragon2d.players[x].selected_shot==1){
          //cold.innerHTML = `trico8`;
            if(ldb==0){                                                                                        
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'red');
              crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.160,'white');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'red'); 
              crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,3.338 ,'white'); 
            }else if(ldb==1){
              //>>> 1 
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'red');
              crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy, 1.45,'white');

              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'red');
              crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,2.765,'white');
            }

      }else if(mb==17 && dragon2d.players[x].selected_shot==1){
            //cold.innerHTML = `grub8`;
            if(ldb==0){                                                                                           
              //<<< 0
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'red');
               crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.315,'white');

            }else if(ldb==1){
              //>>> 1
              crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'blue');
              crearCirculo(xvelocidad2,yvelocidad2,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'black');
              crearCirculo(xvelocidad3,yvelocidad3,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'red');
              crearCirculo(xvelocidad4,yvelocidad4,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,1.945,'white');
              
            }

      }

  }





//.................................



  let poder = parseFloat((velocidadIni * calibrador).toFixed(2));
  let poder2 = parseFloat((velocidadIni2 * calibrador).toFixed(2));
  let poder3 = parseFloat((velocidadIni3 * calibrador).toFixed(2));
  let poder4 = parseFloat((velocidadIni4 * calibrador).toFixed(2));



  //
  //cold.innerHTML = `distanciax:${distanciax} | distanciax2:${distanciax2} | distanciax3:${distanciax3} lado${lado}`;

   
   poderio=actualizarBarra(poder, barraPoderX,rallita,p1);
   poderio2=actualizarBarra(poder2, barraPoderX,rallita2,p2);
   poderio3=actualizarBarra(poder3, barraPoderX,rallita3,p3);
   poderio4=actualizarBarra(poder4, barraPoderX,rallita4,p4);

   shot = parseInt((((100*poderio)/barraPoderX)/100)*400);
   shot2 = parseInt((((100*poderio2)/barraPoderX)/100)*400);
   shot3 = parseInt((((100*poderio3)/barraPoderX)/100)*400);
   shot4 = parseInt((((100*poderio4)/barraPoderX)/100)*400);

   //cold.innerHTML = `tiro: ${shot}`;
 
 };


let poderio=0;
let poderio2=0;
let poderio3=0;
let poderio4=0;

let shot=0;
let shot2=0;
let shot3=0;
let shot4=0;







const actualizarBarra = (power, barraWidh,ralla,nombre) => {
  const linea = power <= 4.00 ? parseInt((power / (barraWidh/100))*barraWidh) : 0;
  if(linea==0 || isNaN(linea)){
    nombre.textContent="";
  }
  ralla.style.left =`${linea}px`;
  nombre.style.left = `${linea+2}px`;
  ralla.style.opacity = '1';

  return linea;
};



let puntox1=0;
let puntoy1=0;
let puntox2=0;
let puntoy2=0;

function formandoLineas(ldb,xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,color,dx,dy,mb){


  let colorcito=color;
   let ti= (2*yvelocidad)/yaceleracion;
    for(let i=0;i<40;i++){

        let bbx = xvelocidad * ((ti) * i / 16) + 0.5 * xaceleracion * Math.pow((ti * i / 16), 2)
        let bby = yvelocidad * ((ti) * i / 16) - 0.5 * yaceleracion * Math.pow((ti * i / 16), 2)

        let bbx2 = xvelocidad * ((ti) * (i+1) / 16) + 0.5 * xaceleracion * Math.pow((ti * (i+1) / 16), 2)
        let bby2 = yvelocidad * ((ti) * (i+1)/ 16) - 0.5 * yaceleracion * Math.pow((ti * (i+1) / 16), 2)

        bbx = bbx / ((800 / pantallaX)/ccc);
        bby = bby / ((600 / pantallaY)/ccc);

        bbx2 = bbx2 / ((800 / pantallaX)/ccc);
        bby2 = bby2 / ((600 / pantallaY)/ccc);  

        if(ldb==1 && mb!=2 && mb!=11){
        puntox1=((bbx) + (dx/ccc));
        puntoy1=((dy/ccc) - (bby));

        puntox2=((bbx2) + (dx/ccc));
        puntoy2=((dy/ccc) - (bby2));

        }else if(ldb==0 && mb!=2 && mb!=11){

        puntox1=(-(bbx) + (dx/ccc));
        puntoy1=((dy/ccc) - (bby));

        puntox2=(-(bbx2) + (dx/ccc));
        puntoy2=((dy/ccc) - (bby2));
        }



        if(ldb==0 && (mb==2 || mb==11)){
        puntox1=((bbx) + (dx/ccc));
        puntoy1=((dy/ccc) - (bby));

        puntox2=((bbx2) + (dx/ccc));
        puntoy2=((dy/ccc) - (bby2));

        }else if(ldb==1 && (mb==2 || mb==11)){

        puntox1=(-(bbx) + (dx/ccc));
        puntoy1=((dy/ccc) - (bby));

        puntox2=(-(bbx2) + (dx/ccc));
        puntoy2=((dy/ccc) - (bby2));
        }



        if(isNaN(puntox1) && isNaN(puntox2) && isNaN(puntoy1) && isNaN(puntoy2)){
          puntox1=0
          puntox2=0;
          puntoy1=0;
          puntoy2=0;
        }


       crearlineas(colorcito, 2, puntox1, puntoy1, puntox2, puntoy2);

  } 


}



function crearCirculo(xvelocidad,yvelocidad,xaceleracion,yaceleracion,pantallaX,pantallaY,ccc,ldb,dx,dy,time,color){


  
    let cx_1 = Math.round(xvelocidad * time + 0.5 * xaceleracion * (time*time));
    let cy_1 = Math.round(yvelocidad * time - 0.5 * yaceleracion * (time*time));


    if(ldb==1){
        cx_1 = cx_1 / ((800 / pantallaX)/ccc);
        cy_1 = cy_1 / ((600 / pantallaY)/ccc);
    }else if(ldb==0){
        cx_1 = -cx_1 / ((800 / pantallaX)/ccc);
        cy_1 = cy_1 / ((600 / pantallaY)/ccc);
    }

        ctx2.beginPath();
        ctx2.ellipse(cx_1 + (dx/ccc), (dy/ccc)-cy_1, 8, 8, 0, 0, 2 * Math.PI);
        ctx2.fillStyle = color; 
        ctx2.fill();
        ctx2.strokeStyle = color; 



}
