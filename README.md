# enentBus
实现vue中的eventBus on,off,once,emit
## 用法：
A页面
```javastript
import EventBus from '****'
export default new EventBus()
```
b页面：
```javastript
import EventBus from 'A'
EventBus.emit('test',9)
```
c页面
```javastript
import EventBus from 'A'
EventBus.on('test',e => {
  console.log(e)
})
```
