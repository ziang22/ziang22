body{
  height: 100vh;
  background: #151515;
  display: grid;
  place-items: center;
  box-sizing: border-box;
}

.heart-loader{
  background: #f44336;
  width: 50px;
  height: 50px;
  position: relative;
  transform: rotate(45deg);
  animation: pulsate 1s infinite;
}

.heart-loader::before,
.heart-loader::after{
  position: absolute;
  content: "";
  display: inline-block;
  width: 50px;
  height: 50px;
  background: #f44336;
  border-radius: 50%;
}

.heart-loader::before{
  top: 0;
  left: -25px;
}

.heart-loader::after{
  top: -25px;
  left: 0;
}

@keyframes pulsate {
  0% {
    transform: rotate(45deg) scale(0.8);
  }
  5% {
    transform: rotate(45deg) scale(0.9);
  }
  10% {
    transform: rotate(45deg) scale(0.8);
  }
  15% {
    transform: rotate(45deg) scale(1);
  }
  50% {
    transform: rotate(45deg) scale(0.8);
  }
  100% {
    transform: rotate(45deg) scale(0.8);
  }
}
