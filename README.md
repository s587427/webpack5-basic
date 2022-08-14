# Webpack5_PRAC

## Webpack 

1. 打包工具編譯成瀏覽器能讀懂的程式碼

2. WebPack可以看做是模块打包机：
    它做的事情是，分析你的项目结构，  找到JavaScript模块以及其它的一些浏览器不能直接运行的拓展语言（Scss，TypeScript等）， 并将其打包为合适的格式以供浏览器使用

3. 安裝 npm i weback webpack-cli webpack-dev-server
    
 > webpack-cli 可以透過命令列來指定相關的配置

 >  webpack-dev-server (熱更新)

### Plugin
* html-webpack-plugin: 
    自動生成script 與link css標籤，也可以客製化html模板(https://github.com/jantimon/html-webpack-plugin#options)

* mini-css-extract-plugin:
    css抽離html
* css-minimizer-webpack-plugin
    壓縮css

### loader **使webpack可以解析不同類型的文件(程式碼)，並轉換回有效模塊**
  * babel-loader
    > 編譯js為瀏覽器可以支援的版本，例如寫es6語法在其他舊瀏覽器中可能不支援故要使用bable-loader來編譯js為舊語法
    
    1. babel-loader 在webpack裡解析，es6的橋樑@babel/core

    2. babel核心模塊 

    3. @babel/preset-env babel預設, 一組babel插件的集合

  * postcss-loader 
    > 處理css網頁的兼容性 (browserslist 設定瀏覽器支援程度) eg:
    >
    >>  moz代表firefox瀏覽器私有屬性
    >
    >>  -ms代表IE瀏覽器私有屬性  
    >
    >>  -webkit代表chrome、safari私有屬性   
    >
    >>  -o代表opera私有屬性

