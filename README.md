# Bronikowski25
Raw results and misc. data for the Bronikowski et al. (2025) paper.

## Paper information

The paper is available on (link), (website). DOI: (doi)

## Data structure

The volumetric results are in the "volumetric_results" directory, further subdivided by survey, while the arc-specific results are in the "arc-specific_results" directory. Additional volumetric method results are available for clusters which fall outside the viewing fields of the surveys, to offer a point of comparison for possible future surveys. **PLEASE CONSULT THE PAPER TO CHECK WHICH CLUSTERS ARE OBSERVABLE TO EITHER SURVEY.**

Files with volumetric results for Rubin's LSST contain the following columns:

- z - redshift bin z, from z-0.05 to z+0.05, in which the results are calculated
- (SN type)_integral - Volumetric SN rate-independent value, N_j / R_j, for the given SN subtype (see paper)
- (SN type)_yield - Volumetric SN yield prediction for the given SN subtype in the redshift bin
- (SN_type)_yield_err - the total uncertainty for the previous value

We provide results for the following subtypes: II (Type IIP and IIL, combined); IIb; IIn; Ia; Ib; Ic; IcBL.

We do not provide in the data files an estimate of the integral's uncertainty, as we assume a flat 30% uncertainty.

Files with volumetric results for Roman's HLTDS are structured similarily, however, they contain separate columns with "wide" and "deep" in column names, indicating the survey tier for which calculations were made.
For Roman, we provide results for the following subtypes: IIP; IIL; IIb; IIn; Ia; Ib; Ic; IcBL.

Files with arc-specific results contain the following columns:

- z - redshift of the image which was assumed in this work. This is spectroscopic, if available, or model derived otherwise;
- Image_ID - ID of the image found in literature
- mu - magnification estimate of the image, either provided in literature directly or estimated from published lens models
- bayes.sfh.sfr - best fit star formation rate (SFR) to this specific image, in units of solar mass/year. This value is not used further if this image's relative uncertainty on SFR and M* was not lowest among all images in the system
- bayes.stellar.m_star - best fit total stellar mass formed (M*) to this specific image, in units of solar mass. This value is not used further if this image's relative uncertainty on SFR and M* was not lowest among all images in the system
- Av - Best fit visual extinction Av
- Cluster - name of the galaxy cluster to which the image belongs
- total_rel_err_best - Sum of relative errors of M* and SFR of the best fit image
- cc_rate - Rate of CC SNe occuring in the lensed galaxy, calculated from the best SFR and M* estimate, in units of yr^-1
- ia_rate - Rate of Ia SNe occuring in the lensed galaxy, calculated from the best SFR and M* estimate, in units of yr^-1
- lsst_(SN_type) - Expected number of SNe of the given type detected by Rubin in its first 3 years of the survey
- roman_(survey_tier)_(SN_type) - Expected number of SNe of the given type detected by Roman, assuming the cluster is observed in the High Latitude Time Domain Survey in the tier given by (survey_tier)
Columns which end with "_err" are error estimates of given values.

Note that we make available additional arc-specific results for clusters which fall outside the viewing fields of the surveys, to offer a point of comparison for possible future surveys. **PLEASE CONSULT THE PAPER TO CHECK WHICH CLUSTERS ARE OBSERVABLE TO EITHER SURVEY.**

