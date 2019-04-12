#### 方法一
                <!DOCTYPE html>
                <html>
                  <head>
                    <meta charset="utf-8" />
                    <title>高度充满父容器</title>
                  </head>
                  <style>
                    .parent {
                      height: 500px;
                      width: 300px;
                      border: 1px solid red;/***/
                      padding: 2px 2px;/***/
                    }

                    .nav {
                      height: 100px;
                      width: 100%;/*必须沾满宽度防止浮动*/
                      float: left;/*必须*/
                      background-color: red;
                    }

                    .content {
                      height:100%;/*必须*/
                      background-color: green;
                    }
                  </style>

                  <body>

                    <div class="parent">
                      <div class="nav">
                        固定高度
                      </div>
                      <div class="content">
                        自适应父容器, 充满剩余的空间 
                      </div>
                    </div>

                  </body>

                </html>
#### 方法二 flex 
     .box {
        display: flex;
        flex-direction: column;
        box-flex: 1;
        height: 100%;
     }
