Download Link: https://assignmentchef.com/product/solved-ee440-assignment-5-frequency-domain-noise-filtering
<br>
<h1> Frequency domain noise filtering</h1>

You are given a noisy image (5_1.bmp) which is affected by noise. Figure 1 shows the noisy image, magnitude and phase of its frequency components. The noise appears in the frequency domain as the white specks highlighted in red. Figure 1: (a) Noisy image (b) magnitude of noisy image’s frequency components (c) phase of noisy image’s frequency components

Perform filtering in the frequency domain to remove the noise. Show the denoised image, and the magnitude and phase components of its DFT coefficients (similar to those in Figure 1).

<strong><em><u>HINTS</u> </em></strong>

<ol>

 <li>You may use this code to find magnitude and phase of an image’s frequency components:</li>

</ol>

<table width="0">

 <tbody>

  <tr>

   <td width="422">im = imread(‘5_1.bmp’); im = double(im); %% apply FFT  f = fftshift(fft2(im)); magnitudeF = log(abs(f)); magnitudeF = mat2gray(magnitudeF); angleF = angle(f); </td>

  </tr>

 </tbody>

</table>




<ol>

 <li>Plot the magnitude and phase of the given noisy image. Use the “data cursor” tool in the Matlab Figure Window to identify the “abnormal” frequency components that are likely to be noise (e.g., the white specks in Figure 1).</li>

</ol>

<ul>

 <li>In order to filter noise, set the above identified frequency components to zero. Due to the symmetrical properties of the DFT, you need to set all the four noise frequency components to 0.</li>

</ul>














