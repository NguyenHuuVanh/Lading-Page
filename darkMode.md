<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tailwincss</title>
    <link rel="stylesheet" href="./dist/output.css" />  
    <link rel="stylesheet" href="./src/app.css">
    <script
      type="module"
      src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"
    ></script>
    <script
      nomodule
      src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.js"
    ></script>
  </head>
  <body>
<label for="toogle" class=" inline-block cursor-pointer toogle-switch">
    <input type="checkbox" name="" id="toogle" class="darkmode-input hidden">
    <div class="w-[100px] h-[50px] rounded-full border border-[#ccc] fixed bottom-5 right-5 p-[5px] z-50 transition-colors">
    <div class="spin h-[38px] w-[38px] rounded-full bg-[#eee]"></div>
    </div>
</label>
    <div class="mx-auto max-w-[1200px] grid grid-cols-4 gap-x-5 p-5">
        <div class="px-5 py-8 rounded-lg border border-[#eee] bg-[#8EC5FC] dark:bg-[#2c3e50] transition-colors">
            <div>
                <img src="https://free3dicon.com/wp-content/uploads/2022/10/perspective_matte-42-264x264.png" alt=""
                class="mb-5">
                <h3 class="text-lg text-center font-semibold mb-5 dark:text-white">Reacomendation</h3>
                <p class="text-sm text-gray-600 text-center leading-loose dark:text-white">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsam aspernatur sit repudiandae animi illo iusto optio ipsa est magni, numquam voluptatum tenetur quasi. Earum voluptate maiores quam voluptatum! Quibusdam, qui.</p>
            </div> 
        </div>

        <div class="px-5 py-8 rounded-lg border border-[#eee] bg-[#8EC5FC] dark:bg-[#2c3e50] transition-colors">
            <div>
                <img src="https://free3dicon.com/wp-content/uploads/2022/10/perspective_matte-47-264x264.png" alt=""
                class="mb-5">
                <h3 class="text-lg text-center font-semibold mb-5 dark:text-white">Reacomendation</h3>
                <p class="text-sm text-gray-600 text-center leading-loose dark:text-white">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsam aspernatur sit repudiandae animi illo iusto optio ipsa est magni, numquam voluptatum tenetur quasi. Earum voluptate maiores quam voluptatum! Quibusdam, qui.</p>
            </div> 
        </div>

        <div class="px-5 py-8 rounded-lg border border-[#eee] bg-[#8EC5FC] dark:bg-[#2c3e50] transition-colors">
            <div>
                <img src="https://free3dicon.com/wp-content/uploads/2022/10/perspective_matte-35-264x264.png" alt=""
                class="mb-5">
                <h3 class="text-lg text-center font-semibold mb-5 dark:text-white">Reacomendation</h3>
                <p class="text-sm text-gray-600 text-center leading-loose dark:text-white">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsam aspernatur sit repudiandae animi illo iusto optio ipsa est magni, numquam voluptatum tenetur quasi. Earum voluptate maiores quam voluptatum! Quibusdam, qui.</p>
            </div> 
        </div>

        <div class="px-5 py-8 rounded-lg border border-[#eee] bg-[#8EC5FC] dark:bg-[#2c3e50] transition-colors">
            <div>
                <img src="https://free3dicon.com/wp-content/uploads/2022/10/perspective_matte-32-264x264.png" alt=""
                class="mb-5">
                <h3 class="text-lg text-center font-semibold mb-5 dark:text-white">Reacomendation</h3>
                <p class="text-sm text-gray-600 text-center leading-loose dark:text-white">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsam aspernatur sit repudiandae animi illo iusto optio ipsa est magni, numquam voluptatum tenetur quasi. Earum voluptate maiores quam voluptatum! Quibusdam, qui.</p>
            </div> 
        </div>
    </div>
    
    <script>
        const toogleSwitch=document.querySelector(".toogle-switch input[type=checkbox]");
        const currentTheme=localStorage.getItem("theme")
        console.log("🚀 ~ file: index.html:112 ~ currentTheme:", currentTheme)
        if(currentTheme){
            document.documentElement.setAttribute("class", currentTheme)
            if(currentTheme==="dark"){
                toogleSwitch.checked=true;
            }
        }
        const switchTheme =(e)=>{
            if(e.target.checked){
                document.documentElement.setAttribute("class","dark")
                localStorage.setItem("theme","dark")
            }
            else{
                document.documentElement.setAttribute("class","light")
                localStorage.setItem("theme","light")
            }
        }
        toogleSwitch.addEventListener("change",switchTheme)
    </script>
  </body>
</html>
