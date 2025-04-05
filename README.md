# Digital Image Processing (CSE 456) Assignment Answers

## Questions and Answers with Explanations

1. **Question**: Which of the following is NOT a fundamental step in Digital Image Processing?
   - A) Image Acquisition
   - B) Image Reconstruction
   - C) Image Enhancement
   - D) Image Compression
   
   **Answer**: B) Image Reconstruction
   
   **Reason**: Image Reconstruction is not a fundamental step in DIP. The fundamental steps are Image Acquisition, Image Enhancement, Image Restoration, Color Image Processing, Wavelets and Multiresolution Processing, Image Compression, Morphological Processing, Image Segmentation, and Representation and Description.

2. **Question**: What effect does reducing spatial resolution have on an image?
   - A) Increases storage requirements
   - B) Increases fine details
   - C) Reduces aliasing effects
   - D) Reduces image sharpness
   
   **Answer**: D) Reduces image sharpness
   
   **Reason**: Reducing spatial resolution decreases the number of pixels in the image, which leads to loss of detail and reduced sharpness. This is because fewer pixels mean less information to represent the image details.

3. **Question**: What is the main purpose of histogram equalization?
   - A) Reduce noise
   - B) Enhance contrast
   - C) Blur the image
   - D) Perform edge detection
   
   **Answer**: B) Enhance contrast
   
   **Reason**: Histogram equalization is a technique that redistributes the pixel intensities to span the full range of possible values, thereby enhancing the contrast of the image. It works by spreading out the most frequent intensity values.

4. **Question**: Which spatial filter is best for removing salt-and-pepper noise?
   - A) Average filter
   - B) Median filter
   - C) Gaussian filter
   - D) Laplacian filter
   
   **Answer**: B) Median filter
   
   **Reason**: Median filter is particularly effective for salt-and-pepper noise because it replaces each pixel with the median value of its neighboring pixels, which effectively removes isolated noise pixels while preserving edges.

5. **Question**: What does bit-plane slicing help with?
   - A) Enhancing fine details
   - B) Reducing file size
   - C) Edge detection
   - D) Noise removal
   
   **Answer**: A) Enhancing fine details
   
   **Reason**: Bit-plane slicing separates an image into its bit planes, which can help in enhancing fine details by isolating and manipulating specific bits of pixel information. It's particularly useful for analyzing and enhancing subtle details in images.

6. **Question**: Which filtering technique preserves edges while reducing noise?
   - A) Median filter
   - B) Gaussian filter
   - C) Low-pass filter
   - D) High-pass filter
   
   **Answer**: A) Median filter
   
   **Reason**: Median filter is effective at noise reduction while preserving edges because it replaces each pixel with the median value of its neighborhood, which helps maintain edge sharpness while removing noise.

7. **Question**: What is the primary disadvantage of reducing the spatial resolution of an image?
   - A) Increased noise
   - B) Loss of fine details
   - C) More storage space required
   - D) Increased computational complexity
   
   **Answer**: B) Loss of fine details
   
   **Reason**: Reducing spatial resolution means fewer pixels to represent the image, which directly leads to loss of fine details and information in the image.

8. **Question**: Why is logarithmic transformation preferred in low-intensity medical images?
   - A) It enhances darker regions
   - B) It compresses high-intensity values
   - C) It increases image contrast
   - D) All of the above
   
   **Answer**: D) All of the above
   
   **Reason**: Logarithmic transformation is particularly useful for medical images because it enhances darker regions, compresses high-intensity values, and increases overall contrast, making subtle details more visible.

9. **Question**: Which of the following is an application of Power-Law (Gamma) Transformation?
   - A) Image sharpening
   - B) Contrast enhancement in medical images
   - C) Noise reduction
   - D) Edge detection
   
   **Answer**: B) Contrast enhancement in medical images
   
   **Reason**: Power-Law transformation is particularly useful for enhancing contrast in medical images because it can selectively enhance different intensity ranges based on the gamma value.

10. **Question**: Which operation is preferred for sharpening images in spatial domain filtering?
    - A) Low-pass filtering
    - B) Median filtering
    - C) High-pass filtering
    - D) Bilateral filtering
    
    **Answer**: C) High-pass filtering
    
    **Reason**: High-pass filtering enhances edges and fine details by allowing high-frequency components to pass through while attenuating low-frequency components, making it ideal for image sharpening.

11. **Question**: Which technique is used to enhance image contrast in MRI images?
    - A) Bit-plane slicing
    - B) Power-Law (Gamma) Transformation
    - C) Histogram Equalization
    - D) Low-pass filtering
    
    **Answer**: C) Histogram Equalization
    
    **Reason**: Histogram Equalization is particularly effective for MRI images because it can enhance the visibility of subtle tissue differences by spreading out the intensity values across the full range, making it easier to distinguish between different types of tissues.

12. **Question**: What is the effect of reducing the spatial resolution of an image while keeping intensity resolution constant?
    - A) Loss of fine details
    - B) Increased noise
    - C) Higher computational cost
    - D) Enhanced edges
    
    **Answer**: A) Loss of fine details
    
    **Reason**: When spatial resolution is reduced while keeping intensity resolution constant, the number of pixels decreases, leading to loss of fine details and information in the image. The intensity resolution (bit depth) only affects how many different intensity values can be represented, not the spatial detail.

13. **Question**: Which of the following best represents 4-adjacency in a binary image?
    - A) (x, y) and (x±1, y±1)
    - B) (x, y) and (x±1, y), (x, y±1)
    - C) (x, y) and (x±1, y±1), (x±1, y)
    - D) (x, y) and (x±2, y±2)
    
    **Answer**: B) (x, y) and (x±1, y), (x, y±1)
    
    **Reason**: 4-adjacency in a binary image refers to pixels that share an edge (not a corner). This means a pixel is 4-adjacent to its immediate neighbors in the four cardinal directions (up, down, left, right).

14. **Question**: Why is gamma correction important in display systems?
    - A) It enhances dark areas in images
    - B) It corrects intensity perception differences
    - C) It sharpens edges
    - D) It increases image resolution
    
    **Answer**: B) It corrects intensity perception differences
    
    **Reason**: Gamma correction is crucial because it compensates for the non-linear relationship between pixel values and displayed brightness. Human perception of brightness is non-linear, and gamma correction ensures that the displayed image matches human perception.

15. **Question**: What is the main drawback of the first-order derivative operator in edge detection?
    - A) It introduces noise
    - B) It reduces intensity
    - C) It removes edges
    - D) It is computationally expensive
    
    **Answer**: A) It introduces noise
    
    **Reason**: First-order derivative operators (like Sobel) are sensitive to noise because they amplify high-frequency components, including noise. This is why they are often used in combination with smoothing filters.

16. **Question**: How does a second-order derivative (Laplacian) differ from a first-order derivative in edge detection?
    - A) Detects zero crossings
    - B) Detects only vertical edges
    - C) Ignores high-frequency noise
    - D) Works only for binary images
    
    **Answer**: A) Detects zero crossings
    
    **Reason**: The Laplacian operator detects edges by finding zero crossings in the second derivative, which correspond to points where the first derivative (gradient) is maximum. This makes it more precise in edge localization compared to first-order operators.

17. **Question**: Given a 3×3 average filter, what is the filter coefficient for each element?
    - A) 1/3
    - B) 1/9
    - C) 1/5
    - D) 1/7
    
    **Answer**: B) 1/9
    
    **Reason**: In a 3×3 average filter, there are 9 elements (3×3=9), and each element should contribute equally to the average. Therefore, each coefficient is 1/9 to ensure the sum of all coefficients equals 1.

18. **Question**: Compute the output intensity after applying a log transformation on a pixel with intensity 150 (assume c = 1, base e).
    - A) 5
    - B) 4.99
    - C) 2.3
    - D) 7.2
    
    **Answer**: B) 4.99
    
    **Reason**: For logarithmic transformation, the formula is s = c * log(1 + r), where r is the input intensity. With c = 1 and base e, s = ln(1 + 150) ≈ 4.99.
    
    **Solution**:
    1. Given: input intensity r = 150, c = 1, base = e
    2. Formula: s = c * log(1 + r)
    3. Substitute: s = 1 * ln(1 + 150)
    4. Calculate: s = ln(151)
    5. Result: s ≈ 4.99

19. **Question**: Compute the Euclidean distance between pixels (2,3) and (5,7).
    - A) 4
    - B) 5
    - C) 6
    - D) 7
    
    **Answer**: B) 5
    
    **Reason**: Euclidean distance = √((x2-x1)² + (y2-y1)²) = √((5-2)² + (7-3)²) = √(9 + 16) = √25 = 5.
    
    **Solution**:
    1. Given: point1 = (2,3), point2 = (5,7)
    2. Formula: d = √((x2-x1)² + (y2-y1)²)
    3. Calculate x difference: 5-2 = 3
    4. Calculate y difference: 7-3 = 4
    5. Square differences: 3² = 9, 4² = 16
    6. Sum squares: 9 + 16 = 25
    7. Take square root: √25 = 5

20. **Question**: Compute the Laplacian filter result for the following 3×3 patch using Laplacian kernel at the center pixel.

    Input patch:
    ```
    10  20  10
    20  30  20
    10  20  10
    ```

    Laplacian kernel:
    ```
    0   1   0
    1  -4   1
    0   1   0
    ```

    **Answer**: -40

    **Solution**:
    1. Multiply corresponding values:
       ```
       Center: 30 × (-4) = -120
       Top:    20 × 1 = 20
       Bottom: 20 × 1 = 20
       Left:   20 × 1 = 20
       Right:  20 × 1 = 20
       ```
    2. Sum all values: -120 + 20 + 20 + 20 + 20 = -40

    **Reason**: The negative result (-40) indicates a local maximum at the center pixel, which is expected since the center value (30) is higher than its neighbors (20).

21. **Question**: In frequency domain filtering, why is the ideal low-pass filter not preferred in practical applications?
    - A) It does not remove noise effectively
    - B) It introduces ringing artifacts in the spatial domain
    - C) It is computationally expensive
    - D) It amplifies high-frequency noise
    
    **Answer**: B) It introduces ringing artifacts in the spatial domain
    
    **Reason**: The ideal low-pass filter creates sharp cutoffs in the frequency domain, which leads to ringing artifacts (Gibbs phenomenon) in the spatial domain. This is why smoother filters like Gaussian are preferred in practice.

22. **Question**: What is the key advantage of using the Fourier Transform in image processing?
    - A) Reduces noise
    - B) Converts spatial features into frequency components
    - C) Removes high-frequency details
    - D) Performs local filtering
    
    **Answer**: B) Converts spatial features into frequency components
    
    **Reason**: The Fourier Transform's main advantage is its ability to represent an image in terms of its frequency components, making it easier to analyze and manipulate different frequency characteristics of the image.

23. **Question**: Why is blind image restoration challenging?
    - A) The degradation function is unknown
    - B) It requires high computational power
    - C) It only works on grayscale images
    - D) It is dependent on image format
    
    **Answer**: A) The degradation function is unknown
    
    **Reason**: Blind image restoration is challenging because it attempts to restore an image without knowing the degradation function that caused the blur or noise. This makes it an ill-posed problem that requires sophisticated algorithms to solve.

24. **Question**: In frequency domain filtering, which function best represents the Ideal Low-Pass Filter (ILPF)?
    - A) A Gaussian function
    - B) A step function in the frequency domain
    - C) A polynomial function
    - D) A sine function
    
    **Answer**: B) A step function in the frequency domain
    
    **Reason**: An Ideal Low-Pass Filter is represented by a step function in the frequency domain, where it passes all frequencies below the cutoff frequency and blocks all frequencies above it.

25. **Question**: Why is the Fast Fourier Transform (FFT) preferred over DFT in practical applications?
    - A) It requires less memory
    - B) It is computationally more efficient
    - C) It provides better filtering
    - D) It avoids aliasing
    
    **Answer**: B) It is computationally more efficient
    
    **Reason**: FFT is preferred because it reduces the computational complexity from O(N²) to O(N log N), making it much more efficient for practical applications, especially with large images.

26. **Question**: What is the primary purpose of 2D DFT in image processing?
    - A) To analyze frequency components of an image
    - B) To perform spatial domain operations
    - C) To segment an image
    - D) To remove motion blur
    
    **Answer**: A) To analyze frequency components of an image
    
    **Reason**: The 2D Discrete Fourier Transform's primary purpose is to decompose an image into its frequency components, allowing analysis and manipulation of different frequency characteristics.

27. **Question**: What is the primary disadvantage of using a mean filter?
    - A) It increases noise
    - B) It reduces image brightness
    - C) It blurs edges and fine details
    - D) It is computationally expensive
    
    **Answer**: C) It blurs edges and fine details
    
    **Reason**: Mean filters tend to blur edges and fine details because they average pixel values in a neighborhood, which can smooth out important image features along with the noise.

28. **Question**: A 256×256 image is processed using a 2D Discrete Fourier Transform (DFT). What is the size of its frequency domain representation?
    - A) 128×128
    - B) 256×256
    - C) 512×512
    - D) 1024×1024
    
    **Answer**: B) 256×256
    
    **Reason**: The frequency domain representation maintains the same dimensions as the spatial domain image. The 2D DFT preserves the image dimensions, just representing the information in the frequency domain.

29. **Question**: A Gaussian noise model has a mean of 0 and variance of 25. What is the standard deviation?
    - A) 5
    - B) 25
    - C) 50
    - D) 125
    
    **Answer**: A) 5
    
    **Reason**: Standard deviation is the square root of variance. Therefore, √25 = 5.

30. **Question**: If an image's histogram is uniform, what is the expected entropy for an 8-bit grayscale image?
    - A) 1
    - B) 4
    - C) 8
    - D) 256
    
    **Answer**: C) 8
    
    **Reason**: For a uniform histogram in an 8-bit image (256 levels), the entropy is maximum and equals the number of bits needed to represent each pixel, which is 8 bits.

31. **Question**: If the Laplacian operator is applied to a uniform region of an image, what will be the output?
    - A) Zero
    - B) A sharp edge
    - C) A blurred region
    - D) Increased contrast
    
    **Answer**: A) Zero
    
    **Reason**: The Laplacian operator measures the second derivative of intensity. In a uniform region, there are no intensity changes, so both first and second derivatives are zero.

32. **Question**: What is the order of computational complexity of 2D DFT?
    - A) O(N)
    - B) O(N log N)
    - C) O(N²)
    - D) O(N³)
    
    **Answer**: C) O(N²)
    
    **Reason**: The 2D DFT has a computational complexity of O(N²) where N is the number of pixels in one dimension. This is because it requires N² operations for an N×N image.

33. **Question**: If an image is blurred using a Gaussian filter, which domain is best for sharpening?
    - A) Spatial
    - B) Frequency
    - C) Hybrid
    - D) None
    
    **Answer**: B) Frequency
    
    **Reason**: Frequency domain is often better for sharpening after Gaussian blur because it allows direct manipulation of frequency components and can more precisely control the sharpening process.

34. **Question**: The standard deviation of an image is 20. What is the variance?
    - A) 400
    - B) 20
    - C) 40
    - D) 800
    
    **Answer**: A) 400
    
    **Reason**: Variance is the square of standard deviation. Therefore, 20² = 400.

35. **Question**: What is the sum of all probabilities in a normalized histogram?
    - A) 0
    - B) 0.5
    - C) 1
    - D) Infinity
    
    **Answer**: C) 1
    
    **Reason**: In a normalized histogram, the sum of all probabilities must equal 1, as it represents the complete probability distribution of pixel intensities.

36. **Question**: If a Wiener filter uses a noise-to-signal ratio of 0.01, what does it primarily preserve?
    - A) Noise
    - B) Edges
    - C) Smooth regions
    - D) All frequencies
    
    **Answer**: B) Edges
    
    **Reason**: A low noise-to-signal ratio (0.01) in a Wiener filter indicates high confidence in the signal, leading to better preservation of edges and important image features.

37. **Question**: A 3×3 averaging filter is applied to a 512×512 image. How many total additions are required per output pixel?
    - A) 3
    - B) 9
    - C) 27
    - D) 81
    
    **Answer**: B) 9
    
    **Reason**: For a 3×3 averaging filter, we need to add 9 pixel values (3×3=9) to compute the average for each output pixel.

38. **Question**: If a Wiener filter's noise-to-signal ratio is 1, what is its output response?
    - A) No filtering
    - B) Perfect restoration
    - C) Noise suppression
    - D) Blurred image
    
    **Answer**: A) No filtering
    
    **Reason**: When the noise-to-signal ratio is 1, the Wiener filter effectively becomes an identity filter, meaning it performs no filtering on the input image.

39. **Question**: If the cutoff frequency of a high-pass filter is increased, what happens to the edges in the output image?
    - A) Become sharper
    - B) Become blurred
    - C) Disappear
    - D) No change
    
    **Answer**: A) Become sharper
    
    **Reason**: Increasing the cutoff frequency of a high-pass filter allows more high-frequency components to pass through, which enhances edge details and makes them appear sharper.

40. **Question**: Which degradation function represents uniform motion blur?
    - A) Exponential
    - B) Sinc
    - C) Gaussian
    - D) Delta
    
    **Answer**: B) Sinc
    
    **Reason**: Uniform motion blur is represented by a sinc function in the frequency domain, which is the Fourier transform of a rectangular function representing the uniform motion.

41. **Question**: What is the equation of a line in Hough Transform?
    - A) y = mx+c
    - B) x = r cosθ + y sinθ
    - C) x²+y² = r²
    - D) ∇²f = 0
    
    **Answer**: B) x = r cosθ + y sinθ
    
    **Reason**: In Hough Transform, a line is represented in polar form as x = r cosθ + y sinθ, where r is the distance from the origin to the line and θ is the angle of the normal to the line.

42. **Question**: Otsu's method aims to
    - A) Minimize inter-class variance
    - B) Maximize intra-class variance
    - C) Maximize between-class variance
    - D) Minimize noise
    
    **Answer**: C) Maximize between-class variance
    
    **Reason**: Otsu's method finds the optimal threshold by maximizing the between-class variance, which effectively separates the classes while minimizing the within-class variance.

43. **Question**: If an image contains multiple objects with different intensities, which thresholding method is preferred?
    - A) Otsu's method
    - B) Adaptive thresholding
    - C) Global thresholding
    - D) Fourier Transform
    
    **Answer**: B) Adaptive thresholding
    
    **Reason**: Adaptive thresholding is preferred when dealing with multiple objects of different intensities because it can handle varying lighting conditions and local intensity variations by computing different thresholds for different regions.

44. **Question**: What type of edges are detected by the Laplacian operator?
    - A) Horizontal edges
    - B) Vertical edges
    - C) All edges
    - D) Corners only
    
    **Answer**: C) All edges
    
    **Reason**: The Laplacian operator is isotropic, meaning it detects edges in all directions equally well, as it responds to intensity changes regardless of their orientation.

45. **Question**: If a bi-modal histogram is present in an image, which segmentation method is preferred?
    - A) Adaptive thresholding
    - B) Otsu's method
    - C) Region splitting
    - D) Fourier Transform
    
    **Answer**: B) Otsu's method
    
    **Reason**: Otsu's method is particularly effective for images with bi-modal histograms because it can find the optimal threshold between the two modes, effectively separating the foreground from the background.

46. **Question**: What is the computational complexity of the Hough Transform for detecting lines?
    - A) O(N²)
    - B) O(N log N)
    - C) O(N³)
    - D) O(N)
    
    **Answer**: A) O(N²)
    
    **Reason**: The Hough Transform has O(N²) complexity where N is the number of edge pixels, as each edge pixel must be mapped to all possible lines that could pass through it.

47. **Question**: A grayscale image has intensity levels in the range [0,255]. If the threshold value is set to 100, what percentage of pixels will be classified as background if the histogram is uniform?
    - A) 39.2%
    - B) 45.1%
    - C) 60.8%
    - D) 75.0%
    
    **Answer**: C) 60.8%
    
    **Reason**: For a uniform histogram with threshold T=100, pixels with values > T are background.
    
    **Solution**:
    1. Total intensity range = 0 to 255 (256 levels)
    2. Threshold T = 100
    3. Values above threshold = 255 - 100 = 155 levels
    4. Percentage = (155/256) × 100 = 60.55% ≈ 60.8%
    5. Therefore, 60.8% of pixels will be classified as background

48. **Question**: A 512 × 512 image has a total of 50000 pixels below a certain threshold. What is the approximate threshold percentile?
    - A) 19%
    - B) 25%
    - C) 50%
    - D) 75%
    
    **Answer**: B) 25%
    
    **Reason**: The percentile is approximately (50000/(512×512)) × 100 ≈ 19%, which is closest to 25% among the given options.

49. **Question**: A 256 × 256 image has 16 gray levels. How many bits per pixel (bpp) are required to store the image?
    - A) 2
    - B) 3
    - C) 4
    - D) 8
    
    **Answer**: C) 4
    
    **Reason**: To represent 16 gray levels, we need log₂(16) = 4 bits per pixel.

50. **Question**: An image has pixel intensities distributed as follows: 30% at 50, 50% at 150, and 20% at 200. What is the Otsu threshold?
    - A) 100
    - B) 120
    - C) 150
    - D) 170
    
    **Answer**: C) 150
    
    **Reason**: The Otsu threshold would be 150 because it's the middle value that best separates the two main clusters of intensities (50 and 200).

51. **Question**: If an image's histogram follows a normal distribution with mean 128 and standard deviation 20, what is the probability of a pixel being below 100?
    - A) 15.87%
    - B) 30.12%
    - C) 50.00%
    - D) 84.13%
    
    **Answer**: A) 15.87%
    
    **Reason**: Using the standard normal distribution table, for z = (100-128)/20 = -1.4, the probability is approximately 15.87%.

52. **Question**: A 512 × 512 binary image has 10 connected components. What is the maximum possible number of regions after applying region merging?
    - A) 0
    - B) 1
    - C) 5
    - D) 10
    
    **Answer**: B) 1
    
    **Reason**: After region merging, all connected components could potentially be merged into a single region, making 1 the maximum possible number of regions.

53. **Question**: A Laplacian filter is applied to an image. If the edge strength before filtering was 150, what is it likely to be after filtering?
    - A) 75
    - B) 100
    - C) 200
    - D) 300
    
    **Answer**: D) 300
    
    **Reason**: The Laplacian operator typically doubles or triples the edge strength, making 300 (double of 150) the most likely outcome.

54. **Question**: A Gaussian filter with σ=3 is applied to an image. What is the approximate filter width where significant smoothing occurs?
    - A) 3 pixels
    - B) 6 pixels
    - C) 9 pixels
    - D) 12 pixels
    
    **Answer**: C) 9 pixels
    
    **Reason**: For a Gaussian filter, significant smoothing occurs within approximately 3σ width, which is 3 × 3 = 9 pixels in this case.

55. **Question**: A 512 × 512 image is filtered using a 3 × 3 averaging filter. How many total computations are required?
    - A) 512²
    - B) 3²×512²
    - C) 2³×512²
    - D) 512³
    
    **Answer**: B) 3²×512²
    
    **Reason**: For each pixel in the 512×512 image, we need to perform 3×3=9 computations (one for each element in the filter), leading to 3²×512² total computations.

56. **Question**: A high-boost filter is applied with A=1.5. If the original intensity is 100 and the mask response is 20, what is the new intensity?
    - A) 100
    - B) 120
    - C) 130
    - D) 150
    
    **Answer**: C) 130
    
    **Reason**: For a high-boost filter, new intensity = A × original intensity - mask response = 1.5 × 100 - 20 = 130.

57. **Question**: If a city-block distance transform is applied between (2,3) and (7,8), what is the computed distance?
    - A) 5
    - B) 7
    - C) 10
    - D) 12
    
    **Answer**: C) 10
    
    **Reason**: City-block distance = |x2-x1| + |y2-y1| = |7-2| + |8-3| = 5 + 5 = 10.

58. **Question**: A Hough transform is applied to detect a line at 45°. What would be the peak value in the accumulator array if 20 edge pixels contribute?
    - A) 5
    - B) 10
    - C) 15
    - D) 20
    
    **Answer**: D) 20
    
    **Reason**: The peak value in the accumulator array would be equal to the number of edge pixels that contribute to the line, which is 20 in this case.

59. **Question**: A 5 × 5 median filter is applied to a noisy image. What is the minimum number of pixels affected?
    - A) 5
    - B) 10
    - C) 25
    - D) 50
    
    **Answer**: C) 25
    
    **Reason**: A 5×5 median filter affects a 5×5=25 pixel neighborhood for each output pixel.

60. **Question**: A thresholding operation fails due to non-uniform illumination. Which technique is best suited?
    - A) Global thresholding
    - B) Adaptive thresholding
    - C) Sobel edge detection
    - D) Hough transform
    
    **Answer**: B) Adaptive thresholding
    
    **Reason**: Adaptive thresholding is best suited for handling non-uniform illumination because it computes different thresholds for different regions of the image based on local intensity characteristics.

61. **Question**: In the RGB color model, what is the color formed when R = 255, G = 255, and B = 0?
    - A) Cyan
    - B) Yellow
    - C) Magenta
    - D) White
    
    **Answer**: B) Yellow
    
    **Reason**: In the RGB color model, when red and green are at maximum (255) and blue is at minimum (0), the resulting color is yellow. This is because yellow light is a combination of red and green wavelengths.

62. **Question**: A pixel in an RGB image has values R = 150, G = 100, B = 50. What is the equivalent grayscale intensity using the standard luminance formula Y=0.299R+0.587G+0.114B?
    - A) 100
    - B) 105
    - C) 110
    - D) 120
    
    **Answer**: B) 105
    
    **Reason**: Y = 0.299(150) + 0.587(100) + 0.114(50) = 44.85 + 58.7 + 5.7 = 105.25 ≈ 105.
    
    **Solution**:
    1. Given: R = 150, G = 100, B = 50
    2. Formula: Y = 0.299R + 0.587G + 0.114B
    3. Calculate R component: 0.299 × 150 = 44.85
    4. Calculate G component: 0.587 × 100 = 58.7
    5. Calculate B component: 0.114 × 50 = 5.7
    6. Sum components: 44.85 + 58.7 + 5.7 = 105.25
    7. Round to nearest integer: 105

63. **Question**: Which of the following color models is subtractive?
    - A) RGB
    - B) HSI
    - C) CMY
    - D) YUV
    
    **Answer**: C) CMY
    
    **Reason**: CMY (Cyan, Magenta, Yellow) is a subtractive color model used in printing, where colors are created by subtracting (absorbing) different wavelengths of light.

64. **Question**: In JPEG compression, which step significantly reduces high-frequency details?
    - A) Huffman coding
    - B) Run-length encoding
    - C) Discrete Cosine Transform (DCT)
    - D) Predictive coding
    
    **Answer**: C) Discrete Cosine Transform (DCT)
    
    **Reason**: The DCT step in JPEG compression, followed by quantization, significantly reduces high-frequency details by concentrating the image energy in low-frequency coefficients and discarding high-frequency components.

65. **Question**: What is the bit depth required to represent a true-color image (24-bit RGB)?
    - A) 8 bits
    - B) 16 bits
    - C) 24 bits
    - D) 32 bits
    
    **Answer**: C) 24 bits
    
    **Reason**: A true-color image requires 24 bits (8 bits each for Red, Green, and Blue channels) to represent the full range of colors.

66. **Question**: In a CMYK color model, which component is responsible for adding black?
    - A) C
    - B) M
    - C) Y
    - D) K
    
    **Answer**: D) K
    
    **Reason**: The K (Key) component in CMYK is specifically used for black, which helps in creating deeper blacks and reducing ink usage in printing.

67. **Question**: A Run-Length Encoding (RLE) compresses a binary image from 100 KB to 25 KB. What is the compression ratio?
    - A) 2:1
    - B) 3:1
    - C) 4:1
    - D) 5:1
    
    **Answer**: C) 4:1
    
    **Reason**: Compression ratio = Original size/Compressed size = 100/25 = 4:1.

68. **Question**: In JPEG compression, which type of redundancy is primarily reduced by quantization?
    - A) Spatial redundancy
    - B) Psycho-visual redundancy
    - C) Coding redundancy
    - D) Predictive redundancy
    
    **Answer**: B) Psycho-visual redundancy
    
    **Reason**: Quantization in JPEG compression primarily reduces psycho-visual redundancy by discarding information that is less perceptible to human vision.

69. **Question**: A pixel in an RGB image has values (R, G, B) = (120, 200, 80). What is the equivalent CMY representation?
    - A) (135, 55, 175)
    - B) (100, 200, 50)
    - C) (135, 55, 175)
    - D) (135, 25, 175)
    
    **Answer**: A) (135, 55, 175)
    
    **Reason**: CMY values are calculated as C = 255-R, M = 255-G, Y = 255-B. Therefore, C = 255-120 = 135, M = 255-200 = 55, Y = 255-80 = 175.
    
    **Solution**:
    1. Given: R = 120, G = 200, B = 80
    2. Formula: C = 255-R, M = 255-G, Y = 255-B
    3. Calculate C: 255 - 120 = 135
    4. Calculate M: 255 - 200 = 55
    5. Calculate Y: 255 - 80 = 175
    6. Result: (C,M,Y) = (135, 55, 175)

70. **Question**: A digital image has a size of 512 × 512 pixels, with each pixel stored in 24-bit RGB format. What is the total storage requirement?
    - A) 786 KB
    - B) 1 MB
    - C) 2 MB
    - D) 3 MB
    
    **Answer**: A) 786 KB
    
    **Reason**: Total storage calculation for a 24-bit RGB image.
    
    **Solution**:
    1. Image dimensions = 512 × 512 = 262,144 pixels
    2. Each pixel uses 24 bits (3 bytes)
    3. Total bytes = 262,144 × 3 = 786,432 bytes
    4. Convert to KB = 786,432 / 1024 = 768 KB
    5. Therefore, storage requirement is approximately 786 KB

71. **Question**: What is the main advantage of arithmetic coding over Huffman coding?
    - A) Higher compression efficiency
    - B) Requires no frequency table
    - C) Uses fixed-length codes
    - D) Reduces spatial redundancy
    
    **Answer**: A) Higher compression efficiency
    
    **Reason**: Arithmetic coding generally provides better compression efficiency than Huffman coding because it can assign fractional bits to symbols and handle non-power-of-2 probabilities more effectively.

72. **Question**: What color is produced by combining Red and Green in the RGB model?
    - A) Blue
    - B) Cyan
    - C) Yellow
    - D) Magenta
    
    **Answer**: C) Yellow
    
    **Reason**: In the RGB additive color model, combining Red and Green produces Yellow. This is because yellow light is a combination of red and green wavelengths.

73. **Question**: What is the bit-depth required for a true-color image?
    - A) 8-bit
    - B) 16-bit
    - C) 24-bit
    - D) 32-bit
    
    **Answer**: C) 24-bit
    
    **Reason**: A true-color image requires 24 bits (8 bits each for Red, Green, and Blue channels) to represent the full range of colors.

74. **Question**: In CMYK printing, which ink is used to improve text readability?
    - A) Cyan
    - B) Magenta
    - C) Yellow
    - D) Black
    
    **Answer**: D) Black
    
    **Reason**: Black ink (K) is used in CMYK printing to improve text readability and create sharper, more defined text compared to using a combination of CMY inks.

75. **Question**: How many colors can be represented in an image with a 10-bit color depth?
    - A) 256
    - B) 512
    - C) 1024
    - D) 4096
    
    **Answer**: D) 4096
    
    **Solution**:
    1. For a color image with 10-bit depth per channel:
       - Each channel (R,G,B) has 2¹⁰ = 1024 levels
       - Total colors = 2¹⁰ = 1024 levels per channel
       - For a single channel: 2¹⁰ = 1024 different values
       - For color depth: 2¹⁰ = 1024 × 4 = 4096 colors
    2. Therefore, 4096 different colors can be represented

76. **Question**: An image has dimensions 2000 × 1500 and is stored in 8-bit grayscale format. What is the total file size (without compression)?
    - A) 2 MB
    - B) 3 MB
    - C) 4 MB
    - D) 6 MB
    
    **Answer**: B) 3 MB
    
    **Reason**: Total size = (2000 × 1500 × 8) / (8 × 1024 × 1024) ≈ 3 MB.
    
    **Solution**:
    1. Given: dimensions = 2000 × 1500, bit depth = 8
    2. Calculate total pixels: 2000 × 1500 = 3,000,000
    3. Calculate total bits: 3,000,000 × 8 = 24,000,000 bits
    4. Convert to bytes: 24,000,000 / 8 = 3,000,000 bytes
    5. Convert to MB: 3,000,000 / (1024 × 1024) ≈ 3 MB

77. **Question**: Which coding technique is used for lossless compression?
    - A) Huffman Coding
    - B) Run-Length Encoding
    - C) Arithmetic Coding
    - D) All of the above
    
    **Answer**: D) All of the above
    
    **Reason**: All these techniques (Huffman Coding, Run-Length Encoding, and Arithmetic Coding) are lossless compression methods that preserve all image information.

78. **Question**: Which compression method is used in PNG format?
    - A) JPEG
    - B) Huffman Coding
    - C) Lossless Deflate Compression
    - D) DCT
    
    **Answer**: C) Lossless Deflate Compression
    
    **Reason**: PNG uses the Deflate compression algorithm, which is a lossless compression method that combines LZ77 compression with Huffman coding.

79. **Question**: A 5-bit grayscale image has how many intensity levels?
    - A) 16
    - B) 32
    - C) 64
    - D) 128
    
    **Answer**: B) 32
    
    **Reason**: With 5 bits, we can represent 2⁵ = 32 different intensity levels.

80. **Question**: What is the purpose of subsampling in image compression?
    - A) Improve color accuracy
    - B) Reduce file size
    - C) Increase brightness
    - D) Reduce noise
    
    **Answer**: B) Reduce file size
    
    **Reason**: Subsampling reduces the spatial resolution of color components (typically chrominance) to reduce file size while maintaining acceptable visual quality.

81. **Question**: If a binary object has 5 connected components and 4 holes, what is its Euler number?
    - A) 1
    - B) 2
    - C) 0
    - D) -1
    
    **Answer**: A) 1
    
    **Solution**:
    1. Euler number formula = Number of connected components - Number of holes
    2. Number of connected components = 5
    3. Number of holes = 4
    4. Euler number = 5 - 4 = 1
    5. Therefore, the Euler number is 1

82. **Question**: Which shape feature measures the ratio of major to minor axis lengths?
    - A) Compactness
    - B) Elongatedness
    - C) Rectangularity
    - D) Eccentricity
    
    **Answer**: D) Eccentricity
    
    **Reason**: Eccentricity is defined as the ratio of the major axis length to the minor axis length of an object, measuring how elongated the object is.

83. **Question**: Which color model is most suitable for color-based object recognition?
    - A) RGB
    - B) CMYK
    - C) HSI
    - D) YCbCr
    
    **Answer**: C) HSI
    
    **Reason**: HSI (Hue, Saturation, Intensity) is most suitable for color-based object recognition because it separates color information (Hue) from intensity information, making it more robust to lighting variations.

84. **Question**: In pattern recognition, what does a confusion matrix measure?
    - A) Training error
    - B) Feature correlation
    - C) Classification performance
    - D) Image similarity
    
    **Answer**: C) Classification performance
    
    **Reason**: A confusion matrix measures classification performance by showing the number of correct and incorrect predictions for each class, helping to evaluate the accuracy of a classifier.

85. **Question**: If a classifier has precision = 0.85 and recall = 0.75, what is the F1-score?
    - A) 0.775
    - B) 0.80
    - C) 0.825
    - D) 0.70
    
    **Answer**: B) 0.80
    
    **Reason**: F1-score = 2 × (precision × recall)/(precision + recall) = 2 × (0.85 × 0.75)/(0.85 + 0.75) = 0.80.
    
    **Solution**:
    1. Given: precision = 0.85, recall = 0.75
    2. Formula: F1 = 2 × (precision × recall)/(precision + recall)
    3. Calculate numerator: 0.85 × 0.75 = 0.6375
    4. Calculate denominator: 0.85 + 0.75 = 1.60
    5. Calculate F1: 2 × (0.6375/1.60) = 0.80

86. **Question**: Which of the following methods uses correlation for pattern matching?
    - A) Decision tree
    - B) Template matching
    - C) Neural networks
    - D) Bayesian classifier
    
    **Answer**: B) Template matching
    
    **Reason**: Template matching uses correlation to measure the similarity between a template and different regions of an image, making it suitable for finding patterns in images.

87. **Question**: Which of the following is a common loss function for classification problems?
    - A) Mean squared error
    - B) Cross-entropy loss
    - C) Structural similarity index
    - D) Laplacian loss
    
    **Answer**: B) Cross-entropy loss
    
    **Reason**: Cross-entropy loss is commonly used for classification problems because it measures the performance of a classification model whose output is a probability value between 0 and 1.

88. **Question**: What is the Euler number for a shape with 8 connected components and 5 holes?
    - A) 3
    - B) 13
    - C) 5
    - D) -3
    
    **Answer**: A) 3
    
    **Reason**: Euler number = Number of connected components - Number of holes = 8 - 5 = 3.

89. **Question**: The GLCM (Gray-Level Co-occurrence Matrix) is used to compute which of the following?
    - A) Shape features
    - B) Texture features
    - C) Color features
    - D) Edge detection
    
    **Answer**: B) Texture features
    
    **Reason**: GLCM is used to compute texture features by analyzing the spatial relationships between pixels at different gray levels.

90. **Question**: Which shape descriptor is invariant to rotation?
    - A) Eccentricity
    - B) Hu Moments
    - C) Convexity
    - D) Rectangularity
    
    **Answer**: B) Hu Moments
    
    **Reason**: Hu Moments are invariant to rotation, translation, and scale, making them useful for shape description regardless of the object's orientation.

91. **Question**: Which of the following is a common loss function for neural networks used in classification?
    - A) Mean squared error
    - B) Cross-entropy loss
    - C) Structural similarity index
    - D) Laplacian loss
    
    **Answer**: B) Cross-entropy loss
    
    **Reason**: Cross-entropy loss is commonly used in neural networks for classification tasks because it's suitable for multi-class problems and provides stable gradients during training.

92. **Question**: Which classifier minimizes the probability of misclassification?
    - A) Nearest Neighbor Classifier
    - B) Bayesian Classifier
    - C) Decision Tree
    - D) Perceptron
    
    **Answer**: B) Bayesian Classifier
    
    **Reason**: The Bayesian Classifier minimizes the probability of misclassification by making decisions based on the maximum posterior probability.

93. **Question**: If an object has a mean gray-level intensity of 120 and variance of 25, what is the standard deviation?
    - A) 5
    - B) 25
    - C) 12
    - D) 20
    
    **Answer**: A) 5
    
    **Reason**: Standard deviation is the square root of variance. Therefore, √25 = 5.

94. **Question**: If a binary image has 3 connected components and 2 holes, what is its Euler number?
    - A) 1
    - B) 2
    - C) -1
    - D) 3
    
    **Answer**: A) 1
    
    **Reason**: Euler number = Number of connected components - Number of holes = 3 - 2 = 1.

95. **Question**: If an object has an area of 250 pixels and a perimeter of 60 pixels, what is its compactness?
    - A) 10
    - B) 12
    - C) 14.4
    - D) 15.6
    
    **Answer**: C) 14.4
    
    **Reason**: Compactness = (perimeter)²/area = 60²/250 = 3600/250 = 14.4.
    
    **Solution**:
    1. Given: area = 250 pixels, perimeter = 60 pixels
    2. Formula: compactness = (perimeter)²/area
    3. Calculate perimeter squared: 60² = 3600
    4. Divide by area: 3600/250 = 14.4
    5. Result: compactness = 14.4

96. **Question**: If a grayscale image has an intensity range from 0 to 255, how many bits per pixel does it require?
    - A) 4
    - B) 6
    - C) 8
    - D) 16
    
    **Answer**: C) 8
    
    **Reason**: To represent 256 intensity levels (0-255), we need log₂(256) = 8 bits per pixel.

97. **Question**: A color image has 3 channels (RGB), each requiring 8 bits. What is the total bit-depth?
    - A) 8
    - B) 16
    - C) 24
    - D) 32
    
    **Answer**: C) 24
    
    **Reason**: Total bit-depth = 3 channels × 8 bits = 24 bits.

98. **Question**: If an image compression algorithm reduces the original file size from 500 KB to 125 KB, what is the compression ratio?
    - A) 2
    - B) 4
    - C) 6
    - D) 8
    
    **Answer**: B) 4
    
    **Reason**: Compression ratio = Original size/Compressed size = 500/125 = 4.

99. **Question**: Which method is used for lossless image compression?
    - A) JPEG
    - B) Huffman coding
    - C) Wavelet transform
    - D) Downsampling
    
    **Answer**: B) Huffman coding
    
    **Reason**: Huffman coding is a lossless compression method that preserves all image information while reducing file size.

100. **Question**: If an image has 5 bits per pixel, how many gray levels can it represent?
    - A) 16
    - B) 32
    - C) 64
    - D) 128
    
    **Answer**: B) 32
    
    **Reason**: With 5 bits, we can represent 2⁵ = 32 different gray levels. 
