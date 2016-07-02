JingRound
=========

Objective-C Version - [here](https://github.com/isaced/JingRound)


Imitation jing.fm music playing view, support rotation and custom parameters.

![image](https://raw.github.com/isaced/JingRound/master/Screenshot.png)

Usage

You can Drag and Drop a UIView in Storybord or Xib,and then change its class `JingRoundView`, set the basic parameter:

```
//Set up a proxy, to get the callback event
self.roundView.delegate = self
//Providing the intermediate image
self.roundView.roundImage = UIImage(named: "girl")
//The initial state, turn or does not turn
self.roundView.isPlay = false
```

Pause and Play:

```
self.roundView.play()
self.roundView.pause()
```

When you touch in the middle of the disc when it will trigger the pause, play events, of course, there is a delegate `JingRoundViewDelegate`:

```
func playStatuUpdate(playState: Bool) {
    NSLog("%@...", playState ? "Playing": "Pause")
}
```

Welcomes feedback：

Author：[http://www.isaced.com/post-210.html](http://www.isaced.com/post-210.html) 
