# pswebpacktranspbundjs_nt
## 6. Using the Future Now
```
module:{
  rules:[
    {
      test:/\.js$/,
      exclude:/(node_modules|bower_components)/,
      use:{
        loader:'babel-loader',
        options:{
          presets:[
            ['@babel/preset-env',{
              debug:true
            }
            
          ]
        }
      }
    }
  ]
}
```
