# FS Sutff


# classes
   path 
   webpack
   awesome-typescript-loader
   awesome-typescript-loader


"lint:auto-fix": "prettier --write './src/**/*.?(ts|tsx|js|scss)' && tslint --fix './src/**/*.?(js|ts|tsx)'"

# tslint

## CLI
https://palantir.github.io/tslint/usage/cli/
## Rules
https://palantir.github.io/tslint/rules/

## typeScript
https://www.tslang.cn/docs/handbook/typescript-in-5-minutes.html

## webPack 
https://webpack.github.io/docs/usage.html
https://webpack.js.org/concepts/

## yarn 
http://qianduan.guru/2016/11/09/yarn-vs-npm/


## react & webpack & typescript
https://www.tslang.cn/docs/handbook/react-&-webpack.html

## is some error could't commit like could't creat .lock file
  use git commit -n  ; skip precommit check 


tslint-config-prettier


# ShortCutKey:

## shell
   ctrl + R  ， 搜索执行过的命令;
   

```js 
/**
 * 加载菜单数据
 * TODO 替换成 Swagger 上的真实接口
 */
const loadMenuData = (): ActionResult =>{
  return [
    {
      types: [
        'MENU_LOAD_DATA',
        'MENU_LOAD_DATA_SUCCESS'
      ],
      credentials: 'omit',
      url: '//rap.alibaba-inc.com/mockjsdata/2004/api/bizunit/allList'
    },
    (dispatch, getState) => {
      const {
        menuDataId
      } = getState().starGraph.starGraph;
      return  dispatch({
        types: [
          'STAR_LOAD_DATA',
          'STAR_LOAD_DATA_SUCCESS'
        ],
        credentials: 'omit',
        url: `//rap.alibaba-inc.com/mockjsdata/2004/api/bizunit/allList?a=${menuDataId}`
      });
    }
  ];
};
```






