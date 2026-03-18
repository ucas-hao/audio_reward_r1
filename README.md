# 📊 Case Studies

---

## Part I: Audio Understanding Preference (AUP)

### 📌 Case 1:
**🎧 Input Context**
* **Prompt:** "How does the prominence of the violin melody change in relation to the female voice throughout the audio clip?"
* **Audio:** `./dataset/wavs/audio_17801.wav`

**🗣️ Candidate Responses**
* **Response 1:** The violin melody is prominent and weaves throughout the instrumental music piece... It starts off with a solo and continues with an animated passage that leads into a lullaby-like section. The violin remains a key element... providing a soothing yet captivating presence.
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

**🎯 Summary**
> **Summary:** Response 2 is the overall winner because it is the only response that actually addresses the prompt's core requirement: comparing the violin to the female voice. Response 1 completely ignores the female voice, failing the prompt entirely. While both models had issues with acoustic grounding (Response 1 missed the voice, Response 2 hallucinated specific instrumental details), Response 2 provided a much more comprehensive answer by acknowledging the speech event at the end of the clip.
* **👑 Overall Winner: Response 2 is better**

<br>

#### 📌 Case 2: [Your Title for AUP Case 2, e.g., Complex Audio Scene Parsing]
*(Template for your second AUP case)*

**🎧 Input Context**
* **Prompt:** "[Insert Prompt Here]"
* **Audio:** `./dataset/wavs/your_audio_2.wav`

**🗣️ Candidate Responses**
* **Response 1:** "[Insert Response 1]"
* **Response 2:** "[Insert Response 2]"

**🧠 Reasoning Chain**

**1. [Dimension 1, e.g., Prompt Following]**
> [Insert reasoning process for this dimension...]
* **🏆 Dimension Winner: [Response 1 / Response 2 / Tie]**

**2. [Dimension 2, e.g., Acoustic Grounding]**
> [Insert reasoning process for this dimension...]
* **🏆 Dimension Winner: [Response 1 / Response 2 / Tie]**

**🎯 Final Verdict**
> **Summary:** [Insert overall reasoning summary...]
* **👑 Overall Winner: [Response X]**

---

### Part II: Audio Generation Preference (AGP)
*This task evaluates the quality, alignment, and acoustic fidelity of generated audio based on a text prompt.*

#### 📌 Case 1: [Your Title for AGP Case 1, e.g., Text-to-Audio Alignment]
**🎧 Input Context**
* **Prompt:** "[Insert Generation Prompt Here, e.g., 'A dog barks three times followed by a car engine starting.']"

**🗣️ Candidate Generations**
* **Response 1 (Audio):** `./dataset/generated/agp_case1_modelA.wav`
* **Response 2 (Audio):** `./dataset/generated/agp_case1_modelB.wav`

**🧠 Reasoning Chain**

**1. Prompt Adherence (Text-to-Audio Alignment)**
> [Insert reasoning: e.g., Response 1 only features two barks, whereas Response 2 correctly captures three distinct barks and the engine sound...]
* **🏆 Dimension Winner: [Response X] is better**

**2. Acoustic Quality (Fidelity & Artifacts)**
> [Insert reasoning: e.g., Response 2 has noticeable high-frequency artifacting and background hiss, while Response 1 presents a clean, studio-quality sound profile...]
* **🏆 Dimension Winner: [Response X] is better**

**🎯 Final Verdict**
> **Summary:** [Insert overall reasoning summary balancing prompt adherence vs. audio quality...]
* **👑 Overall Winner: [Response X]**

<br>

#### 📌 Case 2: [Your Title for AGP Case 2]
*(Template for your second AGP case)*

**🎧 Input Context**
* **Prompt:** "[Insert Prompt Here]"

**🗣️ Candidate Generations**
* **Response 1 (Audio):** `./dataset/generated/agp_case2_modelA.wav`
* **Response 2 (Audio):** `./dataset/generated/agp_case2_modelB.wav`

**🧠 Reasoning Chain**

**1. [Dimension 1]**
> [Insert reasoning process...]
* **🏆 Dimension Winner: [Response 1 / Response 2 / Tie]**

**2. [Dimension 2]**
> [Insert reasoning process...]
* **🏆 Dimension Winner: [Response 1 / Response 2 / Tie]**

**🎯 Final Verdict**
> **Summary:** [Insert overall reasoning summary...]
* **👑 Overall Winner: [Response X]**

---
