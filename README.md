### Hi there 👋

Chances are, you're here from my UniVoice repos. Expand the section below for more info.

<details>
<summary><h3>🗣️🌐🔊 UniVoice stuff</h3></summary>  
  
I'm still working on unifying UniVoice and making it easier to use. To start, I would recommend going through the following repos in my profile:
- 🗣️univoice: the core repo.
- 📱 univoice-samples: a sample chat app made using univoice. This repo currently uses   
- 🎤 univoice-unimic-input: the repo for capturing audio from Microphones, the most common use case  
- 🔉 univoice-audiosource-output: the repo for playing audio using an AudioSource, again the most common usage.  
- 📶 univoice-telepathy-network: a repo for local/WLAN networking for univoice. Basically, you can talk within a local network. Note that again with mobile apps, hosting, network discovery and connecting have some caveats. 
- 🖥️ univoice-mirror-network: a repo for Mirror based networking. If your game or app uses Mirror, the integration is _very_ simple and also runs with dedicated servers.  

Note that:  
- ❌ univoice-airpeer-network is not production suitable. Airpeer, the underlying library is not IL2CPP compatible. It also uses some old WebRTC code where establishing connection tends to fail a lot.
- ❌ airsignal and airpeer are archived repos. Avoid developing with them unless you know your usecase and their limitations well.
- ⚠️ univoice-pun2-network is not production suitable either, but you are welcome to modify it. The core issue (IIRC) was that Photon throttles the amount of data you can send through some custom channels. Since UniVoice doesn't have any sort of audio compression, the size tends to cross the limits very quickly. It did work fine for 2 or 3 participants.

UniVoice has some big improvements lined up, this includes:
- 📦 Most, if not all of the UniVoice related repos moving into the core package, so that you don't have to worry about dependencies. Modules would be activated using scripting define symbols in Unity
- 📱A much better sample scene
- ✍️ Better documentation and maybe even some video tutorials
- 🗣️ Audio compression, echo cancellation, and maybe even encryption (we'll see)
- 🛜 Implementations for Network For GameObjects, PUN2 and maybe also com.unity.webrtc
- 🖥️ Making it more suitable for dedicated server environments. UniVoice was made with peer-to-peer in mind. 

In short, UniVoice is undergoing a lot of changes soon. Those using the repos already would be protected from these changes. It's likely with UniVoice v4, it'll begin a new life with these improvements coming in one by one.

Thanks for the continued support! If you are joining or have been part of the UniVoice journey, give it a Github star ⭐!
  
</details>


  
[![Adrenak's GitHub stats](https://github-readme-stats.vercel.app/api?username=adrenak&count_private=true&theme=dark)](https://github.com/anuraghazra/github-readme-stats)
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
