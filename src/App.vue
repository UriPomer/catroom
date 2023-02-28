<script setup>

</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header> -->

  
    <!--DropDown-->
    <div class="navbar bg-base-300 rounded-box dropdown" style="position: absolute;top:3%; left: 3%; max-width:70%; max-height: 20%" >
        <div class="flex-1 px-2 lg:flex-none" >
          <a class="text-lg font-bold">控制中心</a>
        </div> 
        <div class="flex justify-end flex-1 px-2">
          <div class="flex items-stretch">
            <a class="btn btn-ghost rounded-btn" @onclick="OnClickEvent" >正在开发</a>
            <div class="dropdown dropdown-end" >
              <label tabindex="0" class="btn btn-ghost rounded-btn">功能菜单</label>
              <ul tabindex="0" class="menu dropdown-content p-2 shadow bg-base-100 rounded-box w-52 mt-4">
                <li><a>温控</a></li>
                <li><a>摄像头</a></li>
                <li><a>喂食系统</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    <!--AboutUS-->
    
    <div style="position:absolute; bottom:4%; right: 0%; width:78%; height: 20%" >
        <footer class="footer p-10 bg-base-200 text-base-content" >
          <div>
            <span class="footer-title">Services</span> 
            <a class="link link-hover">广告</a>
          </div> 
          <div>
            <span class="footer-title">Company</span> 
            <a class="link link-hover">关于我们</a> 
            <a class="link link-hover">联系我们</a> 
          </div> 
          <div>
            <span class="footer-title">其他网站</span> 
            <a class="link link-hover">zzz</a> 
            <a class="link link-hover">yyy</a> 
            <a class="link link-hover">xxx</a>
          </div>
        </footer> 
        <footer class="footer px-10 py-4 border-t bg-base-200 text-base-content border-base-300" >
          <div class="items-center grid-flow-col">
            <svg width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd" class="fill-current"><path d="M22.672 15.226l-2.432.811.841 2.515c.33 1.019-.209 2.127-1.23 2.456-1.15.325-2.148-.321-2.463-1.226l-.84-2.518-5.013 1.677.84 2.517c.391 1.203-.434 2.542-1.831 2.542-.88 0-1.601-.564-1.86-1.314l-.842-2.516-2.431.809c-1.135.328-2.145-.317-2.463-1.229-.329-1.018.211-2.127 1.231-2.456l2.432-.809-1.621-4.823-2.432.808c-1.355.384-2.558-.59-2.558-1.839 0-.817.509-1.582 1.327-1.846l2.433-.809-.842-2.515c-.33-1.02.211-2.129 1.232-2.458 1.02-.329 2.13.209 2.461 1.229l.842 2.515 5.011-1.677-.839-2.517c-.403-1.238.484-2.553 1.843-2.553.819 0 1.585.509 1.85 1.326l.841 2.517 2.431-.81c1.02-.33 2.131.211 2.461 1.229.332 1.018-.21 2.126-1.23 2.456l-2.433.809 1.622 4.823 2.433-.809c1.242-.401 2.557.484 2.557 1.838 0 .819-.51 1.583-1.328 1.847m-8.992-6.428l-5.01 1.675 1.619 4.828 5.011-1.674-1.62-4.829z"></path></svg>
            <p>1803A Industries Ltd. <br/>Providing reliable tech since 2023</p>
          </div> 
          <div class="md:place-self-center md:justify-self-end">
            <div class="grid grid-flow-col gap-4">
              <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"></path></svg></a> 
              <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"></path></svg></a>
              <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"></path></svg></a>
            </div>
          </div>
        </footer>
        </div>

        <button class="btn btn-active btn-ghost button"  style="position: absolute; top: 43%; left: 47%; max-height: 10%; " id="CatButton">点我撸猫</button>
        <!--HiddenText-->
        <div tabindex="0" class="collapse collapse-plus border border-base-300 bg-base-100 rounded-box " style="position:absolute; top: 50%; left: 44%; max-height: 10%; max-width:20%;"><font></font>
            <input type="checkbox" /> 
              <div class="collapse-title text-xl font-medium"><font></font>
              点我才能撸猫<font></font>
            </div><font></font>
            <div class="collapse-content"> <font></font>
              <p>你被骗了</p><font></font>
            </div><font></font>
          </div>
        <!--OpenModal-->
            
            <label for="my-modal-3" class="btn" style="position:absolute; top: 36%; left: 47%; max-height: 10%; ">前往撸猫</label>
            <input type="checkbox" id="my-modal-3" class="modal-toggle"/>
            <div class="modal">
            <div class="modal-box relative">
                <label for="my-modal-3" class="btn btn-sm btn-circle absolute right-2 top-2">✕</label>
                <h3 class="text-lg font-bold">想屁吃呢你</h3>
                <p class="py-4">没做完呢</p>
            </div>
            </div>
        
        <!--StuChat-->
        <div style="position: absolute; bottom: 5%; left: 1%; max-width:20%; max-height: 30%" class="stuchat">
            <div class="chat chat-start">
              <div class="chat-bubble chat-bubble-primary">你来这个破网站干嘛？？</div>
            </div>
            <div class="chat chat-end">
              <div class="chat-bubble chat-bubble-secondary">有人告诉我这里可以看猫</div>
            </div>
            <div class="chat chat-start">
              <div class="chat-bubble chat-bubble-accent">那你真是走对地方了，客官里面请</div>
            </div>
            <div class="chat chat-start">
              <div class="chat-bubble chat-bubble-info">我们这有上好的哈工猫给你看</div>
            </div>
            <div class="chat chat-end">
              <div class="chat-bubble chat-bubble-success">什么是哈工猫？？</div>
            </div>
            <div class="chat chat-start">
              <div class="chat-bubble chat-bubble-warning">看来你不属于这里（灭口</div>
            </div>
            <div class="chat chat-end">
              <div class="chat-bubble chat-bubble-error">啊啊啊啊....</div> 
            </div>
        </div>

        <!--BlackBeautifier-->
        <progress class="progress w-56 blackbar" style="position:absolute; top: 5%; right: 3%; max-width:15%"></progress>
        <progress class="progress w-56 blackbar" style="position:absolute; top: 15%; right: 3%; max-width:15%"></progress>
        <progress class="progress w-56 blackbar" style="position:absolute; top: 25%; right: 3%; max-width:15%"></progress>
        <progress class="progress w-56 blackbar" style="position:absolute; top: 35%; right: 3%; max-width:15%"></progress>
        <progress class="progress w-56 blackbar" style="position:absolute; top: 45%; right: 3%; max-width:15%"></progress>
        <progress class="progress w-56 blackbar" style="position:absolute; top: 55%; right: 3%; max-width:15%"></progress>

        <!--ThemeChanger-->
        <div style="position: absolute; bottom:38%; left: 5%;">
            <select data-choose-theme>
                <option value="dark">Dark</option>
                <option value="winter">Light</option>
                <option value="cupcake">Cupcake</option>
                <option value="autumn">Autumn</option>
                <option value="cyberpunk">Cyberpunk</option>
                <option value="retro">Retro</option>
                <option value="aqua">Aqua</option>
                <option value="coffee">Coffee</option>
                <option value="valentine">Valentine</option>
            </select>
        </div>
  
</template>

<style scoped>

</style>
