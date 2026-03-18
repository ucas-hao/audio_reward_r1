# 📊 Case Studies

---

## Part I: Audio Understanding Preference (AUP)

### 📌 Case 1:
**🎧 Input Context**
* **Prompt:** How does the prominence of the violin melody change in relation to the female voice throughout the audio clip?
* **Audio:** `./wavs/audio_17801.wav`

**🗣️ Candidate Responses**
* **Response 1:** The violin melody is prominent and weaves throughout the instrumental music piece, taking center stage at several intervals. It starts off with a solo and continues with an animated passage that leads into a lullaby-like section. The violin remains a key element in this composition, providing a soothing yet captivating presence.
* **Response 2:** The violin melody is initially prominent and central in the music excerpt, taking the lead role in the instrumental ensemble. As the music progresses, the violin's prominence wanes somewhat, giving way to other instruments such as the cello and upright bass which become more audible. Concurrently, the female voice becomes increasingly dominant, eventually overtaking the instrumental sounds by the end of the excerpt.

**🧠 Reasoning Chain**

**1. 🎯Prompt Following** 
> The question specifically asks how the prominence of the violin melody changes in relation to the female voice. Response 1 discusses the violin's prominence but completely fails to mention the female voice at all. It treats the clip as purely instrumental, ignoring a crucial part of the prompt's condition. Response 2 directly addresses the relationship between the violin and the female voice. It notes the violin is initially prominent and then describes how the female voice becomes dominant, overtaking the instruments. This response fully answers the prompt's specific relational question. Therefore, Response 2 followed the instructions, while Response 1 ignored a key constraint.
* **🏆 Dimension Winner: Response 2 is better**.

**2. 🎵Acoustic Grounding** 
> Both models struggle with acoustic grounding for different reasons, leading to a tie in quality for this dimension. Response 1 completely hallucinates the absence of the voice, treating the clip as an instrumental lullaby, which is a major error given the clear speech at the end. However, Response 2, while correctly identifying the voice, also includes significant hallucinations. It claims the violin's prominence wanes to give way to cello and upright bass (which are not clearly audible or dominant in the way described) and implies a gradual transition where the voice becomes increasingly dominant. In reality, the clip is a distinct cut from music to speech, not a gradual overtaking. Because both models fail to accurately describe the specific acoustic reality of the transition—one by missing the speech entirely, and the other by inventing a gradual instrumental fade and specific accompanying instruments—neither can be considered grounded.
* **🏆 Dimension Winner: Tie**.

**3. 📚Comprehensiveness**
> Response 1 is shallow and inaccurate. It misses the most distinct event in the audio clip: the entry of the spoken voice. By ignoring the voice, it fails to provide a comprehensive description of the audio's narrative arc. Response 2 captures the dynamic shift between the musical elements and the spoken word. It provides a more complete picture of the audio event, describing the instrumental introduction and the subsequent entry of the voice. This makes it significantly more comprehensive regarding the actual content of the clip.
* **🏆 Dimension Winner: Response 2 is better** (Significantly more comprehensive regarding actual content).

**⚖️ Summary**
> Response 2 is the overall winner because it is the only response that actually addresses the prompt's core requirement: comparing the violin to the female voice. Response 1 completely ignores the female voice, failing the prompt entirely. While both models had issues with acoustic grounding (Response 1 missed the voice, Response 2 hallucinated specific instrumental details), Response 2 provided a much more comprehensive answer by acknowledging the speech event at the end of the clip.
* **👑 Overall Winner: Response 2 is better**

<br>
<br>

### 📌 Case 2:
**🎧 Input Context**
* **Prompt:** ""
* **Audio:** `./dataset/wavs/audio_17801.wav`

**🗣️ Candidate Responses**
* **Response 1:** 
* **Response 2:** 

**🧠 Reasoning Chain**

**1. 🎯Prompt Following** 
> 
* **🏆 Dimension Winner: Response 2 is better**.

**2. 🎵Acoustic Grounding** 
> 
* **🏆 Dimension Winner: Tie**.

**3. 📚Comprehensiveness**
> 
* **🏆 Dimension Winner: Response 2 is better** (Significantly more comprehensive regarding actual content).

**⚖️ Summary**
> 
* **👑 Overall Winner: Response 2 is better**

---

## Part II: Audio Generation Preference (AGP)


### 📌 Case 3:
**🎧 Input Context**
* **Prompt:** 

**🗣️ Candidate Generations**
* **Audio 1:** `./wavs/audio_387_1.wavv`
* **Audio 2:** `./wavs/audio_387_2.wav`

**🧠 Reasoning Chain**

**1. 🎯Prompt Following** 
> Audio 1 features a piano sound, but the music played is chaotic, atonal, and lacks the structural characteristics typically associated with classical music. It sounds more like random notes being generated rapidly rather than a composed piece. Audio 2 presents a clear, melodic piano performance that strongly resembles the style of classical music, specifically reminiscent of a romantic or classical era piece. It is structured, harmonic, and recognizable as the genre requested.
* **🏆 Dimension Winner: Audio 2 is better**.

**2. 🎵Audio Quality** 
> Audio 1 suffers from significant artifacts. The piano tone is unnatural, warbled, and sounds like a low-bitrate synthesis with phasing issues. The dynamics are flat and unconvincing. Audio 2 has a much cleaner recording quality. The piano sounds realistic, with a natural decay and room ambiance (reverb). While there is some minor tape hiss or background noise, it sounds like a legitimate recording of an instrument rather than a glitchy generation.
* **🏆 Dimension Winner: Audio 2 is better**.

**3. 📚Acoustic Detail**
> Audio 1 lacks acoustic depth; the notes sound plunky and artificial, without the complex resonance of real strings or a piano body. Audio 2 captures the nuances of a piano performance, including the attack of the hammers, the resonance of the strings, and the sustain of the notes. The phrasing and dynamics in Audio 2 provide a much richer acoustic experience.
* **🏆 Dimension Winner: Audio 2 is better**.

**⚖️ Summary**
> Audio 2 is the clear winner across all dimensions. It actually sounds like classical music played on a real piano, adhering perfectly to the prompt. Audio 1 sounds like a garbled, random sequence of synthesized piano notes with poor audio fidelity and no musical structure.
* **👑 Overall Winner: Audio 2 is better**

<br>

### 📌 Case 4:
**🎧 Input Context**
* **Prompt:** 

**🗣️ Candidate Generations**
* **Audio 1:** `./wavs/agp_case1_modelA.wav`
* **Audio 2:** `./wavs/agp_case1_modelA.wav`

**🧠 Reasoning Chain**

**1. 🎯Prompt Following** 
> 
* **🏆 Dimension Winner: Response 2 is better**.

**2. 🎵Audio Quality** 
> 
* **🏆 Dimension Winner: Tie**.

**3. 📚Acoustic Detail**
> 
* **🏆 Dimension Winner: Response 2 is better**.

**⚖️ Summary**
> 
* **👑 Overall Winner: Response 2 is better**
---
