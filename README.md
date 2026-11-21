# TESS-Net: Trust and Event-Edge-Guided State Space Deblurring Network

Ahmad Moori, Vasit Sagan, Omar Tahri, Erik Blasch, and Hadi Ali Akbarpour  
**WACV 2027**

## Introduction

Under fast motion and severe blur, a single RGB observation often loses fine structures and textures, making image-only deblurring fundamentally ill-posed. Event cameras offer complementary high-temporal-resolution measurements during the exposure interval, but effectively exploiting event information remains challenging due to spatially varying reliability and misalignment with blurred image content.

We propose TESS-Net, an event-guided image deblurring network that estimates where event cues are reliable. The network combines structural agreement between RGB and event features with edge evidence from the event stream to produce a pixel-wise trust map. This map guides both event-to-RGB fusion and state updates during horizontal and vertical scans. An Event-Edge Guided Router then combines the two scan outputs according to how closely their edges match those observed by the event camera.

## Network Architecture

![TESS-Net architecture showing trust map estimation, trust-conditioned fusion, and event-edge routing.](figures/architecture.png)
