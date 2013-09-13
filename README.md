## Supports

KRMusicPlayer supports ARC.

## How To Get Started

KRMusicPlayer is using simple methods to control iPod Music Player of iOS.

``` objective-c
- (void)viewDidLoad
{
    [super viewDidLoad];
    KRMusicPlayer *musicPlayer = [KRMusicPlayer sharedManager];
    //播放音樂 ( Play Music )
    [musicPlayer play];
    //停止播放 ( Stop Music )
    [musicPlayer stop];
    //取得歌曲名稱 ( Fetchs Song Name of Playing. )
    NSString *_playingSong = [musicPlayer getPlayingSong];
    //取得專輯名稱 ( Fetchs Album Name of Playing. )
    NSString *_playingAlbum = [musicPlayer getPlayingAlbum];
    //取得歌曲播放時間總長度 ( Fetchs Song Length with Seconds. )
    CGFloat _playingTimeLength = [musicPlayer getPlayingSongDuration];
    //下一首歌 ( Next Song. )
    [musicPlayer nextSong];
    //上一首歌 ( Previous Song. )
    [musicPlayer previousSong];
    //是否正在播放中 ( Music is Playing ? )
    if( musicPlayer.isPlaying )
    {
        // ... 
    }
    
    //是否是暫停播放 ( 或停止播放, Music is Paused ? )
    if( musicPlayer.isPause )
    {
        // ... 
    }
}
```

## Version

KRMusicPlayer now is V0.5 beta.

## License

KRMusicPlayer is available under the MIT license ( or Whatever you wanna do ). See the LICENSE file for more info.
