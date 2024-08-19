<script>
  export default{
    date(){
      return{
        postionY:"",
      }
    },
    methods:{
      postionCange(){
        postionY =  `translateY(${scrollY * 1.4 + 10}px)`;
      },
    }
  }

</script>

<template>
  <div class="Checklist">
    <a href="#topImage"><img src="../../font.png" alt=""></a>
    <a href=""></a>
    <a href=""></a>
  </div>

  <div class="topPage" id="topImage">
    <div class="imgDiv">
      <div class="maskDiv"></div>
    </div>
  </div>

  <div class="preview">

    <p class="recommendFont">　　　產品推薦</p>
    <div class="itemDiv">

      <div class="card" style="width: 18rem;">
        <img src="https://www.ikea.com.tw/dairyfarm/tw/pageImages/page_zh_tw_17103881161672523561.jpeg"
          class="card-img-top" alt="...">
        <div class="card-body">
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/upholstered-chairs/lisabo-art-50561041"><h4 class="card-title fontStyle">LISABO</h4></a>
          <h6 class="fontStyle" style="font-weight: bold">餐椅, 梣木/tallmyra 白色/黑色</h6>
          <p class="card-text fontStyle">布套可以拆下放入機洗，容易清潔

            梣木貼皮和實心樺木為房間營造出充滿暖意、天然的感覺

            梣木是堅固的材質，有著漂亮的紋理， 顏色會隨時間變深，漸漸變成深黃色

            無論你們需要在餐桌上進行哪種活動，這張堅固舒適的餐椅都很合用

            可以搭配LISABO系列內的其他梣木貼皮產品，打造統一風格。</p>
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/upholstered-chairs/lisabo-art-50561041" class="btn btn-primary fontStyle">查看詳情</a>
        </div>
      </div>

      <div class="card" style="width: 18rem;">
        <img src="https://www.ikea.com.tw/dairyfarm/tw/images/commons/1634891076_80400754_S4.webp" class="card-img-top"
          alt="...">
        <div class="card-body fontStyle">
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/non-upholstered-chairs/ronninge-art-80400754"><h4 class="card-title">RÖNNINGE</h4></a>
          <h6 class="fontStyle" style="font-weight: bold">餐椅, 樺木</h6>
          <p class="card-text fontStyle">柔和、圓弧的座椅和椅背，讓你坐得舒適

            木紋清楚可見，可營造自然、溫暖風格

            可搭配多張同顏色的椅子，打造整體風格，或混搭不同顏色的椅子，增添變化

            實心硬木製成，經久耐用。</p>
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/non-upholstered-chairs/ronninge-art-80400754" class="btn btn-primary fontStyle">查看詳情</a>
        </div>
      </div>

      <div class="card" style="width: 18rem;">
        <img src="https://www.ikea.com.tw/dairyfarm/tw/images/799/1079988_PE857792_S4.webp" class="card-img-top"
          alt="...">
        <div class="card-body">
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/non-upholstered-chairs/lisabo-art-80457236"><h4 class="card-title fontStyle">LISABO</h4></a>
          <h6 class="fontStyle" style="font-weight: bold;">餐椅, 梣木</h6>
          <p class="card-text fontStyle">一張穩固的椅子，適用於各類圍繞桌子進行的活動

            梣木飾面和實心樺木給房間帶來溫暖自然的感覺

            梣木是一種堅韌的硬木，表面有漂亮的紋理，經久使用後顏色變深，呈現深黃色

            需要更柔軟的感覺，或要讓房間更具個性？我們備有多種顏色和風格的椅墊以供選擇

            與LISABO系列其他梣木飾面產品使用更一致美觀。</p>
          <a href="https://www.ikea.com.tw/zh/products/dining-seating/non-upholstered-chairs/lisabo-art-80457236" class="btn btn-primary fontStyle">查看詳情</a>
        </div>
      </div>

    </div>
  </div>
  
  <div class="introduceDiv" @scroll="">
    <div class="maskDiv"></div>
  </div>

  <div class="bottomDiv">

  </div>
</template>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=LXGW+WenKai+Mono+TC&display=swap');
@import url('https://fonts.googleapis.com/css2?family=LXGW+WenKai+Mono+TC&family=LXGW+WenKai+TC&display=swap');

body {
  background-color: rgb(238, 238, 193);
}

.topPage {
  width: 100vw;
  height: 70vh;

  .maskDiv {
    width: 100vw;
    height: 70vh;
    backdrop-filter: blur(5px);
  }

  .imgDiv {
    width: 100vw;
    height: 70vh;
    background-image: url("https://www.ikea.com.tw/dairyfarm/tw/pageImages/page_prev_1868_zh_tw_16866744371681051022.jpeg");
    background-repeat: no-repeat;
    background-size: 100% 100%;
  }

}

.Checklist {
  height: 7vh;
  padding: 0 15vw;
  margin: 0 33vw;
  border-radius: 30px;
  position: fixed;
  top: 3%;
  background-color: rgb(184, 226, 159);
  z-index: 1;
}

.preview {
  margin-top: 20vh;

  .itemDiv {
    display: flex;
    flex-wrap: wrap;
  }

  .card {
    margin-left: 15vw;

    .fontStyle {
      font-family: "LXGW WenKai TC", cursive;
      font-weight: 400;
      font-style: normal;
    }

    .card-text{
      height: 15vh;
      overflow:auto;
      text-overflow: ellipsis;
    }
  }

  .card-img-top {
    height: 350px;
  }
}

.recommendFont {
  font-size: 35px;
  margin-bottom: 10vh;
  border-bottom: 2px solid rgb(183, 238, 181);
  font-family: "LXGW WenKai Mono TC", monospace;
  font-weight: 400;
  font-style: normal;
}

.introduceDiv{
  height: 100vh;
  margin-top: 20vh;
  background-image: url(https://s1.1zoom.me/big0/914/Germany_Forests_Trees_493324.jpg);
  background-repeat: no-repeat;
  background-size: 100% 100%;

  .maskDiv {
    width: 100vw;
    height: 100vh;
    backdrop-filter: saturate(200%);
  }
}

.bottomDiv {}
</style>
