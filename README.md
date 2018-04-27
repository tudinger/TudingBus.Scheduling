
车辆调度分配的算法实现
=============================

### [ 算法环境的介绍 ]

```
cd path/to/project

npm install
```

### [ Run tests ] (Comming soon)

```
npm test
```

### [ Start development environment ]

**Start development with webpack-dev-server:**
```
npm run dev
```

### [ Build front for production ]
Build without package.json version change. ex: 3.6.11 -> 3.6.11
```
npm run build
```
Build with main version +1. ex: 3.6.11 -> 4.6.11
```
npm run build-major
```
Build with minor version +1. ex: 3.6.11 -> 3.7.11
```
npm run build-minor
```
Build with patch version +1. ex: 3.6.11 -> 3.6.12
```
npm run build-patch
```

### [ Run node server for production ]

```
npm run start
```

### [ Generate documentations ]

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
