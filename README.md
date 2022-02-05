# my-quick-set-up-tailwind-development-environment
it's a my quick way setup tailwind development environment
```

===============================
1.Start run install (for make folder structur and input.css)
2.instal tailwind moduler
npm i -D tailwindcss postcss autoprefixer
3.inisiasi tailwind
npx tailwind init
4.make router read tail edit tailwind.config.js
   content: ['./public/**/*.{html,js}'],

5.edit package.json for set auto
{
  "scripts": {
  "dev": "npx tailwindcss -i ./src/input.css -o ./public/css/style-dev.css --watch",
  "realese": "npx tailwindcss -o ./public/css/style.css --minify"
  },
6.this setup create index.html you can edit or add html code on "public/index.html" <br>
  if development use style-dev.css down here example code, but if production rewrite style-dev.css to style.css
 : <link  rel="stylesheet" href="./css/style-dev.css"/>  
 
//add here code on body 
  <div class="container items-center mx-auto">
       <nav class="flex justify-between mt-2">
          <div>
            left
          </div>
          <div>
              right
          </div>
       </nav>
       <section></section>
   </div>

7.running
npm run dev
//reasle product
npm run realese


##for test run
npx tailwindcss -i ./src/input.css -o ./public/css/style-dev.css
##this is default run on dark mode if you want change light mode change class html to blank  <html class="dark">
```
