<template>
    <div class="wrapper-headMid" >
      <div class="container">
        <div class="headMid">
            <img class="headMid__logo" src="../assets/Group.png" alt="">
            <button class="headMid__catalog">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <path d="M24 6h-24v-4h24v4zm0 4h-24v4h24v-4zm0 8h-24v4h24v-4z"/>
              </svg>
              <span>Каталог</span>
            </button>
            <div class="headMid__search" >
              <input type="text" placeholder="Хочу найти...">
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <path d="M23.111 20.058l-4.977-4.977c.965-1.52 1.523-3.322 1.523-5.251 0-5.42-4.409-9.83-9.829-9.83-5.42 0-9.828 4.41-9.828 9.83s4.408 9.83 9.829 9.83c1.834 0 3.552-.505 5.022-1.383l5.021 5.021c2.144 2.141 5.384-1.096 3.239-3.24zm-20.064-10.228c0-3.739 3.043-6.782 6.782-6.782s6.782 3.042 6.782 6.782-3.043 6.782-6.782 6.782-6.782-3.043-6.782-6.782zm2.01-1.764c1.984-4.599 8.664-4.066 9.922.749-2.534-2.974-6.993-3.294-9.922-.749z"/>
              </svg>
            </div>
            <div class="headMid__list">
              <svg width="18" height="22" viewBox="0 0 18 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M15 1H3C2.46957 1 1.96086 1.21071 1.58579 1.58579C1.21071 1.96086 1 2.46957 1 3V19C1 19.5304 1.21071 20.0391 1.58579 20.4142C1.96086 20.7893 2.46957 21 3 21H15C15.5304 21 16.0391 20.7893 16.4142 20.4142C16.7893 20.0391 17 19.5304 17 19L17 3C17 1.89543 16.1046 1 15 1V1Z" stroke="#708598" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M12.9999 11.0005H4.99988" stroke="#708598" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M12.9999 15H4.99988" stroke="#708598" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M9.99988 7H7.49988H4.99988" stroke="#708598" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>  
              <span>Список</span>
            </div>
            <div class="headMid__account">
              <span>A</span>
            </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HeadMid',
}
</script>


<style lang="scss">
.wrapper-headMid{
  border-bottom: 2px solid #e3ecf1;
}
.headMid{
  height: 76px;
  display: flex;
  align-items: center;
  &__catalog{
    width: 116px;
    height: 40px;
    background: #FED83D;
    margin-left: 24px;
    border:none;
    cursor: pointer;
    padding: 0;
    outline: 0;
    border-radius: 4px;
    display: flex;
    align-items: center;
    &:active{
      transform: translateY(1px);
    }
    svg{
      height: 20px;
      width: 20px;
      margin-left: 16px;
    }
    span{
      font-style: normal;
      font-weight: 600;
      font-size: 14px;
      line-height: 24px;
      margin-left: 8px;
    }
  }
  &__logo{
    width: 221px;
    height: 48px;
  }
  &__search{
    position: relative;
    margin-left: 24px;
    input{
      width: 526px;
      height: 40px;
      border: 1px solid #ECEFF1;
      border-radius: 4px;
      padding-left: 14px;
    }
    svg{
      position: absolute;
      top: 10px;
      right: 10px;
      fill: #708598;
      width: 20px;
      height: 20px;
    }
  }
  &__list{
    width: 111px;
    height: 40px;
    background: #FAFBFC;
    margin-left: 24px;
    border: 1px solid #ECEFF1;
    position: relative;
    svg{
      position: absolute;
      left: 16px;
      top: 10px;
      width: 16px;
      height: 20px;
    }
    span{
      position: absolute;
      left: 44px;
      top: 8px;
      font-style: normal;
      font-weight: 600;
      font-size: 14px;
      line-height: 24px;
    }
  }
  &__account{
    width: 40px;
    height: 40px;
    background: #9B51E0;
    border-radius: 50%;
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    margin-left: 24px;
    span{
      color: #fff;
      font-style: normal;
      font-weight: 600;
      font-size: 14px;
      line-height: 24px;
    }
  }
}
</style>
