
<center><font size=4>(Submitted on Interspeech 2025)</font></center>


## 1. Abstract

Dysarthric speech reconstruction (DSR) aims to convert dysarthric speech into comprehensible speech while maintaining the speaker's identity. Despite significant advancements, existing methods often struggle with low speech intelligibility and poor speaker similarity. In this study, we introduce a novel diffusion-based DSR system that leverages a latent diffusion model to enhance the quality of speech reconstruction. Our model comprises: (i) a speech content encoder for phoneme embedding restoration via pre-trained self-supervised learning (SSL) speech foundation models; (ii) a speaker identity encoder for speaker-aware identity preservation by in-context learning mechanism; (iii) a diffusion-based speech generator to reconstruct the speech based on the restored phoneme embedding and preserved speaker identity. Through evaluations on the widely-used UASpeech corpus, our proposed model shows notable enhancements in speech intelligibility and speaker similarity.


## 2. Proposed Model Architecture

<img src="./data/model.png" width="100%">

<style>
  .custom-table {
    border-collapse: collapse;
    width: 100%;}
  .custom-table tr:first-child, .custom-table th:first-child {
    border-top: none;}
  .custom-table tr:first-child, .custom-table th:nth-child(2) {
    border-top: none;}
  .custom-table tr:first-child, .custom-table th:last-child {
    border-top: none;}
  .custom-table th:first-child, .custom-table td:first-child {
    border-left: none;
    border-right: none;}
  .custom-table th:nth-child(2), .custom-table td:nth-child(2) {
    border-left: none;
    border-right: none;}
  .custom-table th:last-child, .custom-table td:last-child {
    border-left: none;
    border-right: none;}
</style>

## 3. Comparison with Different Baseline Systems

3.1.1 **Speaker**: <i><font size=4>M12</font></i> **Text**: <i><font size=4>Left</font></i>  **Original Speech**: <audio controls><source src="./data/M12/Original/M12-left.wav" type="audio/wav"></audio>

<style> td, th {boeder: none!important;} </style>

<table class="custom-table">
  <thead>
  <tr>
    <th>FS2-DSR</th>
    <th>CoLM-DSR</th>
    <th>Diff-DSR</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td><audio controls><source src="./data/M12/FS2-DSR/M12-left.wav" type="audio/wav"></audio></td>
    <td><audio controls><source src="./data/M12/CoLM-DSR/M12-left.wav" type="audio/wav"></audio></td>
    <td><audio controls><source src="./data/M12/Diff-DSR/M12-left.wav" type="audio/wav"></audio></td>
  </tr>
  </tbody>
</table>


