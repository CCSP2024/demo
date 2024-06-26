---
layout: default
---

# Abstract
Although current TTS systems can already achieve human-parity voice quality, they still face a critical challenge: they require sufficient high-quality data of the target speaker, which is particularly scarce for long-form expressive speech synthesis. This paper introduces a novel context-aware voice pretraining model leveraging contrastive learning for expressive Text-to-Speech (TTS) synthesis. The model utilizes a vast amount of contextual voice data without explicit speaker labels, capturing the intricate relationship between context and speech expression. It enables the generation of coherent and expressive speech by integrating cross-modal features of context and speech into the TTS model, particularly beneficial when target speaker data is scarce. For validation, the pretraining model is 1) applied to Context-Speech retrieval tasks for parameter optimization and 2) integrated with a zero-shot TTS system to assess the assistance of learned cross-modal features in expressive TTS modeling. Experiments demonstrate that the pretraining framework is capable of learning effective Context-Speech representations, which significantly contribute to the generation of more expressive speech synthesis.

# Contents
- [Abstract](#abstract)
- [Audio Samples](#audio-samples)
  * [Sentences](#Sentences)
  * [Paragraphs](#Paragraphs)

# Audio Samples

## Sentences

<table align="center">
    <tr><th>Transcript</th><th>Reference</th><th>NS2</th><th>NS2+CCSP</th></tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
            They ventured into the temple, facing intricate puzzles and cunning traps.
        </td>
		<td>
            <audio controls style="width: 150px;"><source src="Samples/Reference/s-1.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-1.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-1.wav"></audio><br>
        </td>
    </tr>
    <tr>
		<td width="60%" style="word-wrap:break-word;">
            People praised their bravery and selflessness.
        </td>
		<td>
            <audio controls style="width: 150px;"><source src="Samples/Reference/s-2.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-2-2.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-2-2.wav"></audio><br>
        </td>
    </tr>
    <tr>
		<td width="60%" style="word-wrap:break-word;">
            Once upon a time, in a small town nestled amidst rolling hills, lived two friends, Alex and Emily. 
        </td>
		<td>
            <audio controls style="width: 150px;"><source src="Samples/Reference/s-3.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-3-2.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-3-2.wav"></audio><br>
        </td>
    </tr>
</table>

## Paragraphs

<table align="center">
    <tr><th>Transcript</th><th>NS2</th><th>NS2+CCSP</th></tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          Under a bruised and brooding sky, Mara pressed against the cold, unyielding stone of the city wall. She could feel the vibrations of marching feet in her bones. The enemy was at the gates, the siege had begun.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/p-1.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/p-1.wav"></audio><br>
        </td>
    </tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          The man chuckled and said, "I can assist you, but on one condition – you must help me complete a task." After a moment's contemplation, they agreed, curious about the man's proposition. He led them through perilous mountain valleys until they arrived at an ancient temple.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/p-2.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/p-2.wav"></audio><br>
        </td>
    </tr>  
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          The man chuckled and said, "I can assist you, but on one condition – you must help me complete a task." After a moment's contemplation, they agreed, curious about the man's proposition. He led them through perilous mountain valleys until they arrived at an ancient temple.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/p-3.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/p-3.wav"></audio><br>
        </td>
    </tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          However, amidst their excitement and greed, the rugged man reappeared, wearing an evil grin. "Thank you for your assistance, but this treasure now belongs to me," he declared. Filled with righteous anger, they gripped the sword and prepared to battle.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/p-4.wav"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/p-4.wav"></audio><br>
        </td>
    </tr>
</table>

## FastSpeech2 Samples

<table align="center">
    <tr><th>Transcript</th><th>FS2</th><th>FS2+CCSP</th></tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          Lawson also evaluated the security hazards at the trade mart on november thirteen.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-1_m.mp3"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-1_m.mp3"></audio><br>
        </td>
    </tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          It was so used for the date of the abolition of the star chamber in the sixteenth charles the first.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-2_m.mp3"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-2_m.mp3"></audio><br>
        </td>
    </tr>  
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          The soviet authorities denied oswald permission.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-3_m.mp3"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-3_m.mp3"></audio><br>
        </td>
    </tr>
    <tr>
        <td width="60%" style="word-wrap:break-word;">
          And therefore approximately one point six seconds after the president was shot in the head.
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2/s-4_m.mp3"></audio><br>
        </td>
        <td>
            <audio controls style="width: 150px;"><source src="Samples/NS2+CCSP/s-4_m.mp3"></audio><br>
        </td>
    </tr>
</table>
