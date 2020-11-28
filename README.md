HEADER.JS :
              import React from 'react'
import './Header.css'

function Header({cname , Price , ratting, image}
) {
    return (
        <div className="Header">
            <div className="bannerimage">
            <img src="manworking.png" alt=""/>
            </div>

            <div className="bubbles">
                <img src="bubble.png"  alt=""/>
                <img src="bubble.png"  alt=""/>
                <img src="bubble.png"  alt=""/>
                <img src="bubble.png"  alt=""/>
                <img src="bubble.png"  alt=""/>

            </div>
            
        </div>
    )
}

export default Header



Header.css : 



                  .Header {
    width: 100%;
    height: 1000px;
    background-image:
    linear-gradient(
      rgb(240, 236, 236), #06c1f0
    );
    justify-content: center;
    margin-bottom: -600px;
}

.bannerimage > img {
    position: absolute;
    margin-top: 200px;
    right: 100px;
    opacity: 1;
}

.bubbles img{
  width: 50px;
  opacity: 0.3;
  animation: bubble 7s linear infinite;

}
.bubbles {
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  position: absolute;
  bottom: 0;
}




           For Bubble Animations :
           
           
           
           @keyframes bubble {

  0%{
    transform: translateY(0);
    opacity:0;
  }
  50%{
    opacity:1;
  }
  70%{
    opacity:1;
  }
  100%{
    transform: translateY(-80vh);
    opacity:0;
  }

}
.bubbles img:nth-child(1){
  animation-delay: 2s;
}
.bubbles img:nth-child(2){
  animation-delay: 4s;
}.bubbles img:nth-child(3){
  animation-delay: 2s;
}.bubbles img:nth-child(4){
  animation-delay: 6s;
}.bubbles img:nth-child(5){
  animation-delay: 2s;
}


                
