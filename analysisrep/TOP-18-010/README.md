# Analysis Repository TOP-18-010
This folder stores the EFT fit ingredients of TOP-18-010 (ttgamma (1l) inclusive and differential cross section measurement).

## Content
   * The gridpacks for these samples are created using the central gridpack generation framework (MG 2.6.5)
   * We use the dim6top model and simulate additional EFT weights for ctZ and ctZI, all other Wilson coefficients are set to 0.
   * We set limits on ctZ and ctZI and use an additional restriction card that removes not-used Wilson coefficients. This is done because the ttgamma cards are computationally expensive and it is close to impossible to simulate EFT weights for all WC. The restriction cards can be found in the cards directories.
   * We simulate the ttgamma signal samples (1l, 2l) with additional weights (see cards/signal).
   * We additionally perform cross checks of the reweighting method in simulating ttgamma (1l) samples at ctZ=-1, ctZ=2, ctZI=-1, ctZI=2 and the SM point and compare the reweighting method to those samples (see cards/crosschecks/).
   * We additionally simulate background samples for the affected backgrounds of single-top + photon in t-channel, s-channel and tW and calculate limits with and without reweighted background events (see cards/background/).
