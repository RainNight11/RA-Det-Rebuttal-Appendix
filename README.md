# Rebuttal Appendix -- RA-Det: Towards Universal Detection of AI-Generated Images via Robustness Asymmetry

## Table 1. 
*Cross-generator generalization results across GAN, diffusion, and additional generators. Models are trained on ProGAN and evaluated on unseen generators. Results show that RA-Det consistently achieves strong performance, particularly on additional generators introduced in the rebuttal.*

*(a) Accuracy (ACC ↑)* 

<table>
  <thead>
    <tr>
      <th rowspan="2">Model</th>
      <th colspan="7">Additional Generators</th>
      <th colspan="16">Original Generators</th>
    </tr>
    <tr>
      <th>SDXL</th><th>SDv3.5</th><th>FLUX</th><th>FLUX1-dev</th><th>Midjourney v6</th><th>Infinity</th><th>VAR</th>
      <th>ProGAN</th><th>StyleGAN</th><th>BigGAN</th><th>CycleGAN</th><th>StarGAN</th><th>GauGAN</th><th>StyleGAN2</th><th>whichfaceisreal</th>
      <th>ADM</th><th>Glide</th><th>SDv1.4</th><th>SDv1.5</th><th>VQDM</th><th>Midjourney</th><th>wukong</th><th>DALLE2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>UnivFD</td>
      <td>55.34</td><td>60.10</td><td>27.50</td><td>38.99</td><td>25.12</td><td>66.13</td><td>68.62</td>
      <td>99.81</td><td>80.40</td><td>95.08</td><td>98.33</td><td>95.75</td><td>99.47</td><td>70.76</td><td>86.09</td>
      <td>67.46</td><td>63.09</td><td>63.66</td><td>63.49</td><td>86.01</td><td>56.13</td><td>70.93</td><td>50.75</td>
    </tr>

  <tr>
    <td>NPR</td>
    <td>48.23</td><td>43.60</td><td>47.85</td><td>53.63</td><td>39.98</td><td>59.52</td><td>39.47</td>
    <td>99.90</td><td>96.06</td><td>83.95</td><td>95.19</td><td>97.17</td><td>80.94</td><td>95.61</td><td>60.60</td>
    <td>70.58</td><td>75.18</td><td>76.81</td><td>70.58</td><td>73.22</td><td>76.61</td><td>74.45</td><td>61.88</td>
  </tr>

  <tr>
    <td>DRCT</td>
    <td>82.87</td><td>80.45</td><td>61.65</td><td>70.52</td><td>50.03</td><td>86.62</td><td>76.98</td>
    <td>100.00</td><td>96.91</td><td>99.40</td><td>99.51</td><td>100.00</td><td>99.51</td><td>96.80</td><td>92.08</td>
    <td>86.53</td><td>92.76</td><td>94.05</td><td>92.34</td><td>95.71</td><td>62.97</td><td>94.09</td><td>84.37</td>
  </tr>

  <tr>
    <td>FerretNet</td>
    <td>83.59</td><td>61.20</td><td>53.00</td><td>80.44</td><td>69.58</td><td>78.38</td><td>77.93</td>
    <td>99.84</td><td>98.65</td><td>94.00</td><td>99.51</td><td>99.08</td><td>93.10</td><td>96.87</td><td>50.40</td>
    <td>95.94</td><td>94.68</td><td>96.64</td><td>96.68</td><td>97.99</td><td>97.69</td><td>96.04</td><td>97.75</td>
  </tr>

  <tr>
    <td><b>RA-Det</b></td>
    <td><b>96.29</b></td><td><b>75.61</b></td><td><b>57.19</b></td><td><b>80.58</b></td><td><b>74.97</b></td><td><b>88.32</b></td><td><b>91.63</b></td>
    <td><b>99.98</b></td><td>94.98</td><td><b>98.35</b></td><td>96.52</td><td><b>99.92</b></td><td><b>99.51</b></td><td>95.54</td><td><b>72.20</b></td>
    <td>88.89</td><td>92.94</td><td>96.50</td><td>96.01</td><td>94.43</td><td>80.04</td><td>95.33</td><td>94.30</td>
  </tr>
  </tbody>
</table>

*(b) Average Precision (AP ↑)* 

<table>
  <thead>
    <tr>
      <th rowspan="2">Model</th>
      <th colspan="7">Additional Generators</th>
      <th colspan="16">Original Generators</th>
    </tr>
    <tr>
      <th>SDXL</th><th>SDv3.5</th><th>FLUX</th><th>FLUX1-dev</th><th>Midjourney v6</th><th>Infinity</th><th>VAR</th>
      <th>ProGAN</th><th>StyleGAN</th><th>BigGAN</th><th>CycleGAN</th><th>StarGAN</th><th>GauGAN</th><th>StyleGAN2</th><th>whichfaceisreal</th>
      <th>ADM</th><th>Glide</th><th>SDv1.4</th><th>SDv1.5</th><th>VQDM</th><th>Midjourney</th><th>wukong</th><th>DALLE2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>UnivFD</td>
      <td>57.42</td><td>71.91</td><td>32.42</td><td>38.10</td><td>33.59</td><td>82.40</td><td>85.05</td>
      <td>100.00</td><td>97.48</td><td>99.27</td><td>99.80</td><td>99.37</td><td>99.98</td><td>97.71</td><td>96.73</td>
      <td>89.80</td><td>83.80</td><td>86.14</td><td>85.84</td><td>96.53</td><td>74.00</td><td>91.07</td><td>63.04</td>
    </tr>

  <tr>
    <td>NPR</td>
    <td>51.02</td><td>43.20</td><td>46.35</td><td>65.99</td><td>42.82</td><td>68.40</td><td>40.71</td>
    <td>99.98</td><td>99.78</td><td>85.59</td><td>98.12</td><td>100.00</td><td>82.97</td><td>99.95</td><td>62.91</td>
    <td>75.08</td><td>83.24</td><td>82.79</td><td>83.80</td><td>77.74</td><td>82.61</td><td>78.17</td><td>71.64</td>
  </tr>

  <tr>
    <td>DRCT</td>
    <td>86.67</td><td>81.67</td><td>62.57</td><td>72.51</td><td>45.73</td><td>92.00</td><td>85.41</td>
    <td>100.00</td><td>96.91</td><td>99.40</td><td>99.51</td><td>100.00</td><td>99.51</td><td>96.80</td><td>92.08</td>
    <td>86.53</td><td>92.76</td><td>94.05</td><td>92.34</td><td>95.71</td><td>62.97</td><td>94.09</td><td>84.37</td>
  </tr>

  <tr>
    <td>FerretNet</td>
    <td>96.461</td><td>64.457</td><td>52.356</td><td>92.826</td><td>78.389</td><td>89.153</td><td>88.297</td>
    <td>100.00</td><td>99.97</td><td>98.04</td><td>99.996</td><td>99.992</td><td>98.906</td><td>99.909</td><td>83.13</td>
    <td>99.359</td><td>98.925</td><td>99.638</td><td>99.638</td><td>99.773</td><td>99.674</td><td>99.356</td><td>99.599</td>
  </tr>

  <tr>
    <td><b>RA-Det</b></td>
    <td>91.34</td><td><b>81.65</b></td><td><b>61.50</b></td><td>88.40</td><td>70.93</td><td>80.09</td><td>84.16</td>
    <td><b>100.00</b></td><td>98.90</td><td><b>99.83</b></td><td>99.47</td><td><b>100.00</b></td><td><b>99.77</b></td><td>99.15</td><td>81.13</td>
    <td>95.07</td><td>97.83</td><td>99.08</td><td>98.92</td><td>98.68</td><td>87.53</td><td>98.33</td><td>98.14</td>
  </tr>
  </tbody>
</table>

*(c) TPR at 1% FPR (↑)* 

<table>
  <thead>
    <tr>
      <th rowspan="2">Model</th>
      <th colspan="7">Additional Generators</th>
      <th colspan="16">Original Generators</th>
    </tr>
    <tr>
      <th>SDXL</th><th>SDv3.5</th><th>FLUX</th><th>FLUX1-dev</th><th>Midjourney v6</th><th>Infinity</th><th>VAR</th>
      <th>ProGAN</th><th>StyleGAN</th><th>BigGAN</th><th>CycleGAN</th><th>StarGAN</th><th>GauGAN</th><th>StyleGAN2</th><th>whichfaceisreal</th>
      <th>ADM</th><th>Glide</th><th>SDv1.4</th><th>SDv1.5</th><th>VQDM</th><th>Midjourney</th><th>wukong</th><th>DALLE2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>UnivFD</td>
      <td>1.58</td><td>15.20</td><td>0.00</td><td>0.16</td><td>0.17</td><td>14.72</td><td>18.89</td>
      <td>99.50</td><td>97.50</td><td>89.20</td><td>98.79</td><td>97.48</td><td>99.58</td><td>78.71</td><td>69.20</td>
      <td>44.40</td><td>52.23</td><td>31.30</td><td>30.10</td><td>66.97</td><td>3.08</td><td>47.58</td><td>9.10</td>
    </tr>

  <tr>
    <td>NPR</td>
    <td>2.51</td><td>0.00</td><td>0.10</td><td>11.24</td><td>2.03</td><td>11.57</td><td>0.67</td>
    <td>8.32</td><td>20.21</td><td>1.50</td><td>6.05</td><td>2.86</td><td>3.25</td><td>0.79</td><td>0.00</td>
    <td>12.92</td><td>31.07</td><td>1.87</td><td>2.66</td><td>6.47</td><td>4.57</td><td>3.92</td><td>27.80</td>
  </tr>

  <tr>
    <td>DRCT</td>
    <td>14.96</td><td>0.93</td><td>0.29</td><td>4.47</td><td>0.05</td><td>24.67</td><td>23.02</td>
    <td>95.00</td><td>74.00</td><td>87.60</td><td>87.70</td><td>95.00</td><td>90.80</td><td>76.10</td><td>67.60</td>
    <td>50.40</td><td>60.70</td><td>65.10</td><td>61.40</td><td>72.30</td><td>15.30</td><td>66.80</td><td>43.00</td>
  </tr>

  <tr>
    <td>FerretNet</td>
    <td>96.44</td><td>0.00</td><td>0.00</td><td>94.07</td><td>48.07</td><td>0.00</td><td>0.00</td>
    <td>99.95</td><td>98.43</td><td>70.80</td><td>74.34</td><td>100.00</td><td>88.26</td><td>94.83</td><td>0.00</td>
    <td>0.00</td><td>0.00</td><td>0.00</td><td>0.00</td><td>0.00</td><td>0.00</td><td>0.00</td><td>0.00</td>
  </tr>

  <tr>
    <td><b>RA-Det</b></td>
    <td><b>58.42</b></td><td><b>29.18</b></td><td><b>6.53</b></td><td><b>33.99</b></td><td><b>11.70</b></td><td><b>46.73</b></td><td><b>36.10</b></td>
    <td><b>100.00</b></td><td><b>91.79</b></td><td><b>99.05</b></td><td><b>93.26</b></td><td><b>100.00</b></td><td><b>99.46</b></td><td><b>89.40</b></td><td><b>64.50</b></td>
    <td><b>54.50</b></td><td><b>84.93</b></td><td><b>72.10</b></td><td><b>69.40</b></td><td><b>80.47</b></td><td><b>17.33</b></td><td><b>70.27</b></td><td><b>71.90</b></td>
  </tr>
  </tbody>
</table>

## Table 2.

*Robustness statistics under different perturbation strengths. We report feature similarity and distance metrics for real and fake images across generators, including cosine similarity, L2 similarity, Euclidean distance, standardized Euclidean distance, and Manhattan distance.*

| Model | Type | Std | Cosine (mean) | Cosine (std) | L2 Sim (mean) | L2 Sim (std) | L2 Dist (mean) | L2 Dist (std) | Std Euclid (mean) | Std Euclid (std) | L1 Dist (mean) | L1 Dist (std) |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| ADM | Real | 0.03 | 0.9751 | 0.0235 | 0.1075 | 0.0373 | 9.5083 | 3.8447 | 31.9855 | 0.0016 | 242.15 | 97.93 |
| ADM | Fake | 0.03 | 0.9263 | 0.0541 | 0.0645 | 0.0244 | 16.4525 | 5.8083 | 31.9856 | 0.0018 | 420.09 | 148.80 |
| ADM | Real | 0.05 | 0.9526 | 0.0430 | 0.0789 | 0.0269 | 13.2142 | 5.0854 | 31.9855 | 0.0016 | 336.85 | 128.93 |
| ADM | Fake | 0.05 | 0.8889 | 0.0742 | 0.0519 | 0.0181 | 20.4217 | 6.6591 | 31.9856 | 0.0018 | 520.38 | 169.11 |
| ADM | Real | 0.10 | 0.8969 | 0.0814 | 0.0538 | 0.0178 | 19.7433 | 7.0842 | 31.9854 | 0.0015 | 501.42 | 178.11 |
| ADM | Fake | 0.10 | 0.8171 | 0.1084 | 0.0397 | 0.0127 | 26.4515 | 7.7099 | 31.9857 | 0.0018 | 674.08 | 197.01 |

| BigGAN | Real | 0.03 | 0.9735 | 0.0243 | 0.1027 | 0.0346 | 9.8524 | 3.7631 | 31.9856 | 0.0018 | 251.80 | 97.61 |
| BigGAN | Fake | 0.03 | 0.8934 | 0.0742 | 0.0534 | 0.0196 | 19.9658 | 6.6823 | 31.9862 | 0.0024 | 508.81 | 169.72 |
| BigGAN | Real | 0.05 | 0.9526 | 0.0398 | 0.0776 | 0.0257 | 13.2901 | 4.8124 | 31.9855 | 0.0016 | 339.81 | 123.26 |
| BigGAN | Fake | 0.05 | 0.8536 | 0.0859 | 0.0442 | 0.0143 | 23.7114 | 6.9084 | 31.9863 | 0.0024 | 605.49 | 175.68 |
| BigGAN | Real | 0.10 | 0.9007 | 0.0744 | 0.0541 | 0.0176 | 19.4517 | 6.6993 | 31.9855 | 0.0015 | 494.83 | 172.64 |
| BigGAN | Fake | 0.10 | 0.8009 | 0.1040 | 0.0371 | 0.0106 | 27.8850 | 7.2102 | 31.9862 | 0.0024 | 710.84 | 183.28 |

| CycleGAN | Real | 0.03 | 0.9710 | 0.0275 | 0.0981 | 0.0321 | 10.2835 | 3.9846 | 31.9855 | 0.0016 | 262.94 | 103.00 |
| CycleGAN | Fake | 0.03 | 0.9181 | 0.0618 | 0.0616 | 0.0213 | 17.1931 | 6.1485 | 31.9856 | 0.0018 | 437.76 | 155.93 |
| CycleGAN | Real | 0.05 | 0.9461 | 0.0447 | 0.0728 | 0.0224 | 14.1219 | 5.0469 | 31.9855 | 0.0016 | 361.62 | 131.08 |
| CycleGAN | Fake | 0.05 | 0.8733 | 0.0841 | 0.0486 | 0.0153 | 21.7135 | 6.9371 | 31.9856 | 0.0018 | 550.64 | 174.63 |
| CycleGAN | Real | 0.10 | 0.8889 | 0.0737 | 0.0498 | 0.0147 | 20.8229 | 6.4330 | 31.9855 | 0.0016 | 529.68 | 162.64 |
| CycleGAN | Fake | 0.10 | 0.7990 | 0.1105 | 0.0373 | 0.0106 | 27.7472 | 7.4712 | 31.9855 | 0.0016 | 702.33 | 186.71 |
