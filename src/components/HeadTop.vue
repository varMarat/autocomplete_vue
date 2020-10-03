<template>
    <div class="wrapper-headTop" >
      <div class="container">
        <div class="headTop">
          <div class="headTop__location">
              <svg fill="#92A2B1" width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M12 10c-1.104 0-2-.896-2-2s.896-2 2-2 2 .896 2 2-.896 2-2 2m0-5c-1.657 0-3 1.343-3 3s1.343 3 3 3 3-1.343 3-3-1.343-3-3-3m-7 2.602c0-3.517 3.271-6.602 7-6.602s7 3.085 7 6.602c0 3.455-2.563 7.543-7 14.527-4.489-7.073-7-11.072-7-14.527m7-7.602c-4.198 0-8 3.403-8 7.602 0 4.198 3.469 9.21 8 16.398 4.531-7.188 8-12.2 8-16.398 0-4.199-3.801-7.602-8-7.602"/>
              </svg>
              <span>Волгоградская область</span>
          </div>
          <div class="headTop__info-menu">
            <a href="#">Тендеры</a>
            <a href="#">База подрядчиков</a>
            <select name="select" id="">
              <option selected>Другие сервисы</option>
              <option>Значение 1</option> 
              <option>Значение 2</option>
              <option>Значение 3</option>
            </select>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HeadTop',
}
</script>


<style lang="scss">
.wrapper-headTop{
    background: #FAFBFC;
    width: 100%;
    height: 32px;
    border-bottom: 1px solid #e3ecf1;
}
.headTop{
  display: flex;
  justify-content: space-between;
  height: 100%;
  &__location{
    display: flex;
    align-items: center;
    cursor: pointer;
    span{
      color:#92A2B1;
      line-height: 20px;
      font-size: 12px;
      font-weight: 400px;
      font-style: normal;
      margin-left: 8px;
    }
  }
  &__info-menu{
    display: flex;
    align-items: center;
    a{
      text-decoration: none;
      cursor: pointer;
      margin-right: 24px;
      font-style: normal;
      font-weight: normal;
      font-size: 12px;
      line-height: 20px;
      color:#92A2B1;
    }
    select{
      border: none;
      font-style: normal; 
      font-weight: normal;
      font-size: 12px;
      line-height: 20px;
      color:#92A2B1;
      background: #FAFBFC;
      cursor: pointer;
      outline: none;
    }
  }
}
</style>
