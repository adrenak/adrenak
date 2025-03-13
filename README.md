## Hi there 👋

[![Adrenak's GitHub stats](https://github-readme-stats.vercel.app/api?username=adrenak&count_private=true&theme=dark)](https://github.com/anuraghazra/github-readme-stats)

Regular UniVoice news will be available [on my blog here](https://blog.vatsalambastha.com/search/label/univoice) if you want to be notified, consider subscribing to [my newsletter](https://vatsalambastha.kit.com/newsletter)

### 🗣️🌐🔊 UniVoice updates  
__Major changes have happened between UniVoice v3 and v4__
* All previously [separate UniVoice repositories](https://github.com/adrenak?tab=repositories&q=univoice&type=&language=&sort=) have been archived and moved to the [main UniVoice repository](https://github.com/adrenak/univoice) in efforts of making it a mono repo. This means no more dealing with a big list of package dependencies (and their dependencies)!  
* Opus codec support has been added via [Concentus-Unity](https://www.github.com/adrenak/concentus-unity). This means your bandwidth usage is <90% compared to v3, making it suitable for production use.
* Mirror is supported out of the box and a sample scene is included to help you get started! 
* Old network implementations for [PUN2](https://github.com/adrenak/univoice-pun2-network), [Telepathy](https://github.com/adrenak/univoice-telepathy-network), [Mirror](https://github.com/adrenak/univoice-mirror-network) and [Airpeer](https://github.com/adrenak/univoice-airpeer-network) currently only work with UniVoice v3. They'll be added as in-built networks to v4 in future releases.

__Changes to dependency repositories:__
* [UniMic](https://github.com/adrenak/unimic) has moved to v3:
  * Multiple mic devices can be used in parallel
  * Major improvements to the API
  * Fixes to the audio frame construction
  * Performance improvements and reduced GC allocation
  * `StreamedAudioSource.cs` for playback of audio frames as they arrive. Runtime changes in frequency, channel count and frame length are handled automatically.

* [Concentus-Unity](https://www.github.com/adrenak/concentus-unity) for pure C# Opus functionality with Speex resampler. 
  * Encoding and decoding features are present in `ContentusEncodeFilter.cs` and `ConcentusDecodeFilter.cs` in the form of incoming and outgoing audio filters.
  * Even through it's C#, building with IL2CPP should help approaching native performance.

* [BRW](https://github.com/adrenak/brw) used for writing and reading binary messages is unchanged.

* [UnityOpus](https://github.com/adrenak/unityopus) for Opus features via interop calls to native libraries (not a dependency, but can be added easily)
  * This _isn't_ a dependency yet. The reason is that the pre-built native libraries in UnityOpus may cause build errors (on Android). Hence the move to Concentus-Unity for a pure C# approach that's build target independent.
  * If you wish to use native libraries for Opus features, import UnityOpus into your project and add [this file](https://github.com/adrenak/univoice/blob/9826982a8e42540f461d53b70f33964c0e01e005/Assets/Adrenak.UniVoice/Runtime/Impl/Filters/OpusFilter.cs) for encode and decode filters.
  * Also if you can get new native libraries built for Windows, Linux, Android, iOS and Mac using the existing C++ code, I'd really appreciate a pull request 😊

__UniVoice has some big improvements lined up, this includes:__
- ✍️ Better documentation and maybe even some video tutorials
- 🗣️ Echo cancellation
- 🛜 Support for FishNet, Purr, Mirage, Network For GameObjects, PUN2 and maybe also Unity WebRTC

Thanks for the continued support! If you are joining or have been part of the UniVoice journey, give it a Github star ⭐!
<!--
**adrenak/adrenak** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
