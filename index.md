<img align="center" src="resources/literally_one_white_pixel.png" style="  display: block; margin-left: auto;
margin-right: auto; width: 0%;" />

This page contains a static and an interactive demo for our approach to controllable artificial speaker embeddings using principal directions.  

## Static Demo
We selected two seed speaker embeddings (one with a feminine and one with a masculine voice) and changed the latents along the principal directions affecting predominantly femininity/masculinity and calmness/arousal of the voice. Some other characteristics, like audio quality, may also be influenced by this. In each setting, we synthesize a long sentence consisting of a concatenation of six smaller but phonetically balanced sentences taken from the Harvard Sentences in [IEEE Recommended Practice for Speech Quality Measurements, 1969](https://ieeexplore.ieee.org/document/1162058).

### Femininity / Masculinity
- <div style="color:darkgreen; display:inline; font-weight: bold;" > Masculine Seed Voice: </div><div style="display:inline;"> The birch canoe slid on the smooth planks, glue the sheet to the dark blue background, it's easy to tell the depth of a well, these days a chicken leg is a rare dish, rice is often served in round bowls, the juice of lemons makes fine punch. <br>  <br> </div>

    <table style='width: 100%;'>
        <tr>
            <td>Seed Voice</td><td><audio controls="" ><source src="resources/femininity_masculinity/m_seed.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Feminine</td><td><audio controls="" ><source src="resources/femininity_masculinity/m_more_fem.wav" type="audio/wav"></audio></td></tr><tr>
            <td><More Towards Feminine/td><td><audio controls="" ><source src="resources/femininity_masculinity/m_most_fem.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Masculine</td><td><audio controls="" ><source src="resources/femininity_masculinity/m_more_masc.wav" type="audio/wav"></audio></td></tr><tr>
            <td>More Towards Masculine</td><td><audio controls="" ><source src="resources/femininity_masculinity/m_most_masc.wav" type="audio/wav"></audio></td></tr><tr>
        </tr>
    </table>

- <div style="color:darkgreen; display:inline; font-weight: bold;" > Feminine Seed Voice: </div><div style="display:inline;"> The source of the huge river is the clear spring, kick the ball straight and follow through, help the woman get back to her feet, a pot of tea helps to pass the evening, smoky fires lack flame and heat, the soft cushion broke the man's fall. <br>  <br> </div>

    <table style='width: 100%;'>
        <tr>
            <td>Seed Voice</td><td><audio controls="" ><source src="resources/femininity_masculinity/f_seed.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Feminine</td><td><audio controls="" ><source src="resources/femininity_masculinity/f_more_fem.wav" type="audio/wav"></audio></td></tr><tr>
            <td><More Towards Feminine/td><td><audio controls="" ><source src="resources/femininity_masculinity/f_most_fem.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Masculine</td><td><audio controls="" ><source src="resources/femininity_masculinity/f_more_masc.wav" type="audio/wav"></audio></td></tr><tr>
            <td>More Towards Masculine</td><td><audio controls="" ><source src="resources/femininity_masculinity/f_most_masc.wav" type="audio/wav"></audio></td></tr><tr>
        </tr>
    </table>

### Calmness / Arousal

- <div style="color:darkgreen; display:inline; font-weight: bold;" > Masculine Seed Voice: </div><div style="display:inline;"> The birch canoe slid on the smooth planks, glue the sheet to the dark blue background, it's easy to tell the depth of a well, these days a chicken leg is a rare dish, rice is often served in round bowls, the juice of lemons makes fine punch. <br>  <br> </div>

    <table style='width: 100%;'>
        <tr>
            <td>Seed Voice</td><td><audio controls="" ><source src="resources/calmness_arousal/m_seed.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Calmness</td><td><audio controls="" ><source src="resources/calmness_arousal/m_more_calmness.wav" type="audio/wav"></audio></td></tr><tr>
            <td><More Towards Calmness/td><td><audio controls="" ><source src="resources/calmness_arousal/m_most_calmness.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Arousal</td><td><audio controls="" ><source src="resources/calmness_arousal/m_more_arousal.wav" type="audio/wav"></audio></td></tr><tr>
            <td>More Towards Arousal</td><td><audio controls="" ><source src="resources/calmness_arousal/m_most_arousal.wav" type="audio/wav"></audio></td></tr><tr>
        </tr>
    </table>

- <div style="color:darkgreen; display:inline; font-weight: bold;" > Feminine Seed Voice: </div><div style="display:inline;"> The source of the huge river is the clear spring, kick the ball straight and follow through, help the woman get back to her feet, a pot of tea helps to pass the evening, smoky fires lack flame and heat, the soft cushion broke the man's fall. <br>  <br> </div>

    <table style='width: 100%;'>
        <tr>
            <td>Seed Voice</td><td><audio controls="" ><source src="resources/calmness_arousal/m_seed.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Calmness</td><td><audio controls="" ><source src="resources/calmness_arousal/m_more_calmness.wav" type="audio/wav"></audio></td></tr><tr>
            <td><More Towards Calmness/td><td><audio controls="" ><source src="resources/calmness_arousal/m_most_calmness.wav" type="audio/wav"></audio></td></tr><tr>
            <td>Towards Arousal</td><td><audio controls="" ><source src="resources/calmness_arousal/m_more_arousal.wav" type="audio/wav"></audio></td></tr><tr>
            <td>More Towards Arousal</td><td><audio controls="" ><source src="resources/calmness_arousal/m_most_arousal.wav" type="audio/wav"></audio></td></tr><tr>
        </tr>
    </table>


## Interactive Demo
The interactive demo contains modification sliders for all principal directions, and options for other properties controlled by the TTS (not in scope of the paper).
<html>
    <script
	    type="module"
	    src="https://gradio.s3-us-west-2.amazonaws.com/3.19.1/gradio.js"
    ></script>

    <gradio-app src="https://flux9665-thisspeakerdoesnotexist.hf.space"></gradio-app>

</html>

