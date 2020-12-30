# Vision and the Atmosphere

Narasimhan and Nayar [IJCV, 2002]

## Method

First exploit two fundamental scattering models, then model the chromatic effects of the atmospheric scattering.

### Mechannisms of Atmospheric Scattering

The radiant intensity $I(\theta, \lambda)$ of the unit volumn in the direction $\theta$ is:

$I(\theta,\lambda) = \beta(\theta,\lambda)E(\lambda)$.

The total flux scattered by this volume is obtained by integrating over the entire sphere:

$\phi(\lambda) = \beta(\lambda)E(\lambda)$,

where $\beta(\lambda)$ is the total scattering coefficient. It represents the ability of the volume to scatter flux of a given wavelength in all directions.

#### Attenuation

$\frac{dE(x,\lambda)}{E(x,\lambda)}=-\beta(\lambda)dx$,

$E(d,\lambda) = E_0(\lambda)e^{-\beta(\lambda)d}$.

#### Airlight

#### Overcast Sky Illumination

#### Depth of Light Sources from Attenuation

$E(d,\lambda) = g \frac{I_0(\lambda)e^{-\beta(\lambda)d}}{d^2}$

The final image brightness recorded is determined as:

$E' = \int{s(\lambda)E(d,\lambda)d\lambda}$.

For the visible light spectrum:

$\beta(\lambda) = \frac{Constant}{\lambda^\gamma}$,

where $\gamma \approx 0$ for fog and dense haze. Then, we have:

$E'=g\frac{e^{-\beta d}}{d^2}I'$.

Now introduce difference in optical thicknesses (DOT), given two different weather conditions:

$R'=\ln{R}=\frac{E_1'}{E_2'}=e^{-(\beta_1-\beta_2)d}$.

Consider two different light sources:

$\frac{R_i'}{R_j'}=\frac{d_i}{d_j}$,

or a more robust version if we take the denominators as Einstein sum.

