# Hyperspectral Imaging notes

---

## [Webinar 1](https://www.youtube.com/watch?v=Z_Zub7wJTFs)

**HSI** _**H**yper**s**pectral **I**maging_, or _chemical/spectroscopic imaging_ : acquiring a spectre info from

**Hypercube**: 3D data struct (2 spatial, 1 wavelength dimension), it can be built according to 3 approaches (whiskbroom scanning, staring imager config, pushbroom acquisition[most used])

<center><img src="https://i.imgur.com/i1bC3rF.png" width=400px></img></center>

**Pushbroom config**: acquisition of simultaneous spectral measurements from a series of adjacent spatial positions. _A relative movement between the object and the detectors is required_

### HSI Based logics, algo and analysis

<center><img src="https://i.imgur.com/i4GXGv8.png" width=500px></img></center>

#### Spectra handling:

#### PCA

### Applications (mainly aggregates)


---

## [Webinar 2](https://www.youtube.com/watch?v=xg2oXcYAZZQ&list=PL8opRgSZuuilix1tUauHaQuIsiYIAUZkk)

**Radiation**:

Bodies emits different energies in different wavelengths.

<center><img src="https://i.imgur.com/7EaY51Y.png" width=500px></img></center>

**Components** :

<center><img src="https://i.imgur.com/AuMul5g.png" width=500px></img></center>

- Emissivity :
  $$ \epsilon $$

- Absorptivity :
  $$ \alpha = \epsilon $$

- Transmittance:
  $$ \tau $$

- Reflectance:
  $$ r $$

We have :
$$\epsilon + \tau + r = 1$$

## What does the camera sees :

<center><img src="https://i.imgur.com/CRoQmL7.png" width=500px></img></center>

### Angle dependence Bidirectional Reflectance Distribution Function:

<center><img src="https://i.imgur.com/lAagz6B.png" width=300px></img></center>

### Domains:

The _reflective_ domain, is dominated by reflected light (ex: what we see is mainly reflection of light)

The _emessive_ domain is dominated by emitted light, because of the green house effect, that block also thermal radiations of the sun to penetrate, so we do not have shadows and things are not really what they are used to.

<center><img src="https://i.imgur.com/aV0twUq.png" width=500px></img></center>

Experience: Your phone camera can detect IR radiations from your remote controler. [cmos sensor].

**Multi/hyper-spectral sensors** are sonsors for multiple wavelengths, where each pixel gives a spectral signature.

**WHY Hyperspectral** :

- Each pixel gives information about the material

### Ways of making multi-hyper-spectral sensor:

- **Mosaic**: Like Bayer filter
- **Multilayer**: stacking multiple sensors hoping that one will pass through the first ones
- **Filter wheel**: one broad band sonsor, and a wheel having multiple filters, each $N^{th}$ image is from band $k$. In a static world, the pixels are **registred** (aligned).
- **Scanning**: scan one line and with imspector optics you get multiple specral values, to scan a scene use a mirror and scan all of it OR move the entire sensor => **pushbroom sensor**.

<center><img src="https://i.imgur.com/uUYIkYB.png" width=500px></img></center>

- **Interferometer**:

<center><img src="https://i.imgur.com/9ZHTfc4.png" width=500px></img></center>

## Applications:

- Ground to ground recon (military)

<center><img src="https://i.imgur.com/zFFBGk9.png" width=500px></img></center>

- Minerological mapping

<center><img src="https://i.imgur.com/9xhhseL.png" width=500px></img></center>

- Disturbed soil

<center><img src="https://i.imgur.com/6mYOsZb.png" width=500px></img></center>

- Night vision devices : **Image enhacers NOT thermal IR**

<center><img src="https://i.imgur.com/WD3WeZL.png" width=500px></img></center>

- Non destructive testing

<center><img src="https://i.imgur.com/HmNfDNh.png" width=500px></img></center>
