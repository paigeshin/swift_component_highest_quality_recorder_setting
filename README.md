# swift_component_highest_quality_recorder_setting

```swift

let audioFilename = getDocumentsDirectory().appendingPathComponent("\(fileName).\(fileExtension)")
let settings = [
        AVFormatIDKey: kAudioFormatAppleLossless,
        AVSampleRateKey: 44100.0,
        AVNumberOfChannelsKey: 2 as NSNumber,
        AVEncoderAudioQualityKey: AVAudioQuality.max.rawValue
] as [String : Any]
    audioRecorder = try! AVAudioRecorder(url: audioFilename, settings: settings)


```
