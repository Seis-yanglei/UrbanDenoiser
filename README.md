# UrbanDenoiser - Denoise for urban seismological noise

We develop a deep-learning-based denoising algorithm, UrbanDenoiser, to filter out urban seismological noise.
The model of UrbanDenoiser is present as 210906-023102.zip, which is trained by a transfer learning from DeepDenoiser (https://github.com/wayneweiqiang/DeepDenoiser), using waveform datasets containing rich noise sources from the urban Long Beach dense array and high signal-to-noise ratio (SNR) earthquake signals from the rural San Jacinto dense array.

With the denoised Long Beach dense array data by UrbanDenoiser, we relocate the seismisity beneath Long Beach, and present the earthquake catalog in LB Catalog_2012_061-067.txt.
The first column is the date, the second column is the number of the three-second window during which the earthquake happened. The third to fifth columns represent the earthquake location in our 3D imaging volume, with the grid spacing of 200 m in each direction (Depth, E-W, N-S). California State Plane Coordinate System Zone 7 is applied here. The origin of the 3D imaging volume represents (1293400 m, 1226000 m, 0 m) in Zone 7. The last column represents the number of median absolute deviation (MAD) the back-projected amplitudes exceeding the detection threshold.

Related paper:
Lei Yang, Xin Liu, Weiqiang Zhu, Liang Zhao, Gregory C. Beroza. 2022. Toward Improved Urban Earthquake Monitoring through Deep-Learning-Based Noise Suppression. Science Advances, DOI: 10.1126/sciadv.abl3564.

