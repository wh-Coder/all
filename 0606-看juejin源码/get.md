- SplashScreen 这个是干什么的？

- 直接写onPress(this._fn) 错误

两种方法改正：在constructor中 this._fn = this._fn.bind(this)

或者改写成onPress(() => {this._fn()})