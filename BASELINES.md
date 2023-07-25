# HL Dataset Baselines
## Introduction
We provide a collection of baselines for the high-level captioning task, consisting in generating **scene, action** and **rationale** description for the image and baselines of the **narrative captiong generation task** using the [HL-Narrative Dataset](https://huggingface.co/datasets/michelecafagna26/hl-narratives) an extension of the [HL Dataset](https://huggingface.co/datasets/michelecafagna26/hl) generating narrative captions based on the three axes.

## HL-scenes

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Model</th>
<th valign="bottom">Cider</th>
<th valign="bottom">SacreBLEU</th>
<th valign="bottom">ROUGE-L</th>
<!-- TABLE BODY -->
<!-- ROW: GIT -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/git-base-captioning-ft-hl-scenes">GIT-base</a></td>
<td align="center">103.00</td>
<td align="center">24.67</td>
<td align="center">33.90</td>
</tr>
<!-- ROW: BLIP -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/blip-base-captioning-ft-hl-scenes">BLIP-base</a></td>
<td align="center">116.00</td>
<td align="center">26.46</td>
<td align="center">35.30</td>
<!-- ROW: ClipCap -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/clipcap-base-captioning-ft-hl-scenes">ClipCap (LM+Mapping)</a></td>
<td align="center">145.00</td>
<td align="center">36.73</td>
<td align="center">42.83</td>
</tr>
</tbody></table>

## HL-actions

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Model</th>
<th valign="bottom">Cider</th>
<th valign="bottom">SacreBLEU</th>
<th valign="bottom">ROUGE-L</th>
<!-- TABLE BODY -->
<!-- ROW: GIT -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/git-base-captioning-ft-hl-actions">GIT-base</a></td>
<td align="center">110.63</td>
<td align="center">15.21</td>
<td align="center">30.43</td>
</tr>
<!-- ROW: BLIP -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/blip-base-captioning-ft-hl-actions">BLIP-base</a></td>
<td align="center">123.07</td>
<td align="center">17.16</td>
<td align="center">32.16</td>
<!-- ROW: ClipCap -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/clipcap-base-captioning-ft-hl-actions">ClipCap (LM+Mapping)</a></td>
<td align="center">176.54</td>
<td align="center">27.37</td>
<td align="center">39.15</td>
</tr>
</tbody></table>

## HL-rationales

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Model</th>
<th valign="bottom">Cider</th>
<th valign="bottom">SacreBLEU</th>
<th valign="bottom">ROUGE-L</th>
<!-- TABLE BODY -->
<!-- ROW: GIT -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/git-base-captioning-ft-hl-rationales">GIT-base</a></td>
<td align="center">42.58</td>
<td align="center">5.90</td>
<td align="center">18.57</td>
</tr>
<!-- ROW: BLIP -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/blip-base-captioning-ft-hl-rationales">BLIP-base</a></td>
<td align="center">46.11</td>
<td align="center">6.21</td>
<td align="center">19.74</td>
<!-- ROW: ClipCap -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/clipcap-base-captioning-ft-hl-rationales">ClipCap (LM+Mapping)</a></td>
<td align="center">78.04</td>
<td align="center">11.71</td>
<td align="center">25.76</td>
</tr>
</tbody></table>

## HL-Narratives

<table><tbody>
<!-- START TABLE -->
<!-- TABLE HEADER -->
<th valign="bottom">Model</th>
<th valign="bottom">Cider</th>
<th valign="bottom">SacreBLEU</th>
<th valign="bottom">ROUGE-L</th>
<!-- TABLE BODY -->
<!-- ROW: GIT -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/git-base-captioning-ft-hl-narratives">GIT-base</a></td>
<td align="center">75.78</td>
<td align="center">11.11</td>
<td align="center">27.61</td>
</tr>
<!-- ROW: BLIP -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/blip-base-captioning-ft-hl-narratives">BLIP-base</a></td>
<td align="center">79.39</td>
<td align="center">11.70</td>
<td align="center">26.17</td>
<!-- ROW: ClipCap -->
<tr><td align="left"><a href="https://huggingface.co/michelecafagna26/clipcap-base-captioning-ft-hl-narratives">ClipCap (LM+Mapping)</a></td>
<td align="center">63.91</td>
<td align="center">8.15</td>
<td align="center">24.53</td>
</tr>
</tbody></table>
