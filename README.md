

 ABSTRACT
 Conversational AI is revolutionizing how humans interact with technology, yet it largely overlooks ethical and cultural contexts. Hiday, an Islamic voice assistant, fills this gap by analyzing spoken conversations in Urdu, identifying ethical breaches such as gossip
 or disrespectful language, and offering corrective feedback in real time. Leveraging advancements in speech-to-text, NLP, and text-to-speech technologies, Hiday embodies Islamic principles to foster better communication habits. It not only identifies but also educates users about ethical speech, acting as a technological tool for self improvement and spiritual growth.
 

 1 PROBLEM STATEMENT
 1.1 Ethical Lapses in Everyday Conversations
 In informal and professional settings, conversational lapses like
 gossip, neglecting greetings, or using foul language are common.
 These behaviors harm relationships, erode trust, and contradict the
 values of respect and morality emphasized in Islam. Despite the
 availability of conversational AI tools, there is no system tailored
 to encourage ethical practices or integrate cultural and religious
 sensitivities into communication.
 1.2 The Need for Hiday
 There is a pressing need for an intelligent system that not only
 processes conversations but also evaluates them against a moral
 framework. Hiday addresses this by providing a proactive, voice
 based solution to guide individuals in practicing Islamic ethical
 principles during conversations.
 
 2 INTRODUCTION
 2.1 Contextual Motivation
 In many cultures, especially Islamic societies, ethical communica
tion is seen as a reflection of character and faith. However, daily
 conversations often stray from these values due to social pressures
 or habits. This behavior, although normalized, is discouraged in
 Islamic teachings, which emphasize avoiding gossip (ghibat), main
taining politeness, and fostering positive social interactions.
 Existing AI tools like Alexa or Siri prioritize functionality—
 setting reminders, fetching information—but lack cultural or ethical
 awareness. Inspired by this gap, Hiday reimagines voice assistants
 as tools for spiritual and moral improvement, combining the capa
bilities of advanced AI with Islamic teachings.
 2.2 Key Innovations of Hiday
 Hiday is not just a tool but a guide. Its key innovations include:
 • Real-time conversational analysis in Urdu, making it acces
sible to a broader audience.
 • Feedback rooted in Islamic ethics, with clear references to
 principles from the Quran and Hadith.
 • Aneducational dimension that explains why certain conver
sational behaviors should be avoided.
 3 RELATE DWORK
 3.1 Advances in Conversational AI
 Conversational AI has rapidly advanced with the introduction of
 systems like GPT-based assistants, multilingual speech-to-text en
gines, and sentiment analysis models. However, these systems focus
 primarily on utility rather than ethics.
 3.2 GapsinExisting Solutions
 Several toolssupportUrduspeechrecognition,includingtheGoogle
 Speech API and open-source tools like CMU Sphinx, but these
 are designed for transcription rather than ethical evaluation. Sim
ilarly, NLP tools like BERT and Hugging Face Transformers
 excel in multilingual text analysis but are not tailored for religious
 or cultural ethics.
 Hidayintegratesthesetechnologiesintoacohesivesystemwhile
 addressing the unique requirements of real-time ethical guidance.
 4 APPROACH
 4.1 System Overview
 Hiday is composed of three primary modules:
 (1) Speech Processing Module: Converts spoken Urdu into
 text.
 (2) NLP Analysis Module: Analyzes transcriptions to detect
 ethical violations.
 (3) Feedback Generation Module: Responds in Urdu with
 corrective guidance.
 These modules are underpinned by advanced tools and algo
rithms, ensuring efficiency and accuracy.
 4.2 Speech Processing
 Tools and Techniques:
 • PyAudio: Captures live audio streams in real-time.
 • GoogleSpeech-to-TextAPI:ConvertsUrduaudiointo text
 with high accuracy (92%).
 Challenges:
 • Accent and Dialect Variations: Addressed using a diverse
 dataset covering multiple accents.
 • Noisy Environments: Filters and denoising algorithms im
prove recognition in group settings.
 4.3 NLPAnalysis
 Core Components:
 (1) Regex-Based Rule Detection: Flags gossip phrases (e.g.,
 kya aap jantay hain ke? (in urdu)
 (2) Named Entity Recognition (NER): Identifies entities to
 f
 lag gossip about specific individuals. Fine-tuned BERT mod
els achieved very high score.
 (3) SentimentAnalysis:Detects negative tones using Hugging
 Face transformers.
 (4) Ethical Violation Scoring: Evaluates the severity of de
tected issues and prioritizes feedback.
 4.4 Feedback Generation
 Tools and Techniques:
 • gTTS(Google Text-to-Speech): Converts ethical feedback
 into spoken Urdu.
 • Personalized Feedback: Friendly yet firm tones ensure
 users are not alienated.
 Example Workflow:
 kya tum nay suna Ali nay larai mai kya kya
 kaha ahmed ko? (in urdu)
 Gheebat say guraiz krain. (in Urdu)
 5 EVALUATIONANDEXPERIMENTS
 5.1 Experimental Setup
 Datasets:
 • Urdu Speech Dataset for training speech-to-text.
 • Curated text dataset for ethical NLP tasks (gossip, swearing
 detection).
 Benchmarks:
 • Trigger: greeting
 • Detected: 1
 • Responded: 1 (100.00
 • Missed Responses: 0 (0.00
 • False Positives (Responded without Detection): 0
 • Trigger: abuse
 • Detected: 3
 • Responded: 3 (100.00
 • Missed Responses: 0 (0.00
 • False Positives (Responded without Detection): 0
 • Trigger: gheebat
 • Detected: 6
 • Responded: 6 (100.00
 • Missed Responses: 0 (0.00
 • False Positives (Responded without Detection): 0
 • ===Performance Metrics ===
 • Total Audio Buffers Processed: 28
 • Recognized Audio: 16 (57.14
 • Unrecognized Audio: 12 (42.86
 • Speech Recognition Errors: 12
 5.2 Results
 User testing showed a 76% positive response rate, with participants
 reporting improved awareness of ethical communication.


EXPLANATION OF MODEL OUTPUTS
 The running outputs of the model in the screenshots can be sum
marized as follows:
 1. Initialization
 • Thesystem calibrates for ambient noise, setting an energy
 threshold to 934.9103721716871.
 • The NamedEntity Recognition (NER) model is loaded.
 2. Speech Recognition
 • The assistant begins listening for input. When valid audio
 input is detected, it transcribes the spoken text into written
 form in Urdu.
 • If the input audio is unclear or contains excessive noise, the
 system outputs:
 Speech Recognition could not understand
 audio.
 3. Response Generation
 • Uponsuccessful transcription, the assistant generates a re
sponse based on the input. Example responses include:
 Gheebat na krain (in urdu)
 • If the assistant is currently speaking, it logs:
 Assistant is currently speaking. Ignoring
 input.
 Additional input during this time is ignored until the current
 response is completed.
 4. Control Handling
 • The system manages multiple iterations of input and output.
 Each cycle involves listening, transcribing, and responding,
 with proper handling of overlapping inputs.

Conclusion
 The outputs showcase a functional speech-to-text and response
 system with clear handling of edge cases, such as noisy input.
