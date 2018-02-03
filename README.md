# pswebpacktranspbundjs_nt

## 6. Using the Future Now
### 9 Do Not Transform Harmony Import
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
            }]            
          ]
        }
      }
    }
  ]
}
```
### 11 Understanding Browserlist Queries
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
              debug:true,
              modules:false,
              targets:{
                browsers:['last 2 chrome versions']
              }
            }
          ]
        }
      }
    }
  ]
}
```
