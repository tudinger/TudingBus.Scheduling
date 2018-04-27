
车辆调度分配的算法实现
=============================

### [ 算法环境的介绍 ]

通过一个算法将订单分配到不同的车辆中（假设车辆属性完全相同，订单除了时间、日期及地点外，其他也都相同）。


### [ 实验数据 ]

此问题实属NP Hard问题，同样的算法去求解不同的数据会有不同的结果。目前此版本简单使用一组数据。

INPUT数据包含
1. 100辆车（车内不含任何订单）
2. 2792个订单，每个订单拥有不同的起始日期、时间，结束日期、时间，起始地点、结束地点

OUTPUT数据包含
1. 100辆车，及每辆车中被分配的订单。

OUTPUT数据文件为scheduledVehiclesOf100FAvV.json, 其中2792个订单被完美分配到了100辆车中，以天为单位计算的车辆使用率为100%



```
npm run doc

// then open the index.html in your browser
google-chrome ./docs/index.html
```

### [ ESLint ]

**Disable the default js inspector in your IDE and active the eslint code quality tool.**

**For running ESLint check on JS files manually:**

```
./node_modules/.bin/eslint path/to/your/file.js

./node_modules/.bin/eslint ./src/**/*.js
```
([Learn more about ESLint command line interface](https://eslint.org/docs/user-guide/command-line-interface))

For more details of current ESLint configurations, check the file ".eslintrc.json".

### [ node server ]
port: 8888
### [ webpack-dev-server ]
port: 9000
### [ webpack BundleAnalyzerPlugin ]
port: 8999




### [ docker build ]
docker login

### [ Publish with Docker ]
1. docker build -t tudingit/tudingitweb:tdbus-client-v353 .
2. docker push tudingit/tudingitweb:tdbus-client-v353
3. goto virtual machine with putty http://51.144.3.152/  ssh tdbus@51.144.3.152
4. sudo docker login
5. sudo docker pull tudingit/tudingitweb:tdbus-client-v353
6. goto web portal to create or config image | http://51.144.3.152:9999/  username: tudingit, pwd: tudingit
