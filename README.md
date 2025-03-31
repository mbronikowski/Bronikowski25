# Bronikowski25
Raw results and misc. data for the Bronikowski et al. (2025) paper.

## Paper information

The paper is available on (link), (website). DOI: (doi)

## Data structure

The volumetric results are in the "volumetric_results" directory, further subdivided by survey, while the arc-specific results are in the "arc-specific_results" directory. Additional volumetric method results are available for clusters which fall outside the viewing fields of the surveys, to offer a point of comparison of possible future surveys. **PLEASE CONSULT THE PAPER TO CHECK WHICH CLUSTERS ARE OBSERVABLE TO EITHER SURVEY.**

Files with volumetric results for Rubin's LSST contain the following columns:

- z - redshift bin z, from z-0.05 to z+0.05, in which the results are calculated

- (SN type)_integral - Volumetric SN rate-independent value, N_j / R_j, for the given SN subtype (see paper)

- (SN type)_yield - Volumetric SN yield prediction for the given SN subtype in the redshift bin

- (SN_type)_yield_err - the total uncertainty for the previous value

We provide results for the following subtypes: II (Type IIP and IIL, combined); IIb; IIn; Ia; Ib; Ic; IcBL.

We do not provide in the data files an estimate of the integral's uncertainty, as we assume a flat 30% uncertainty.

Files with volumetric results for Roman's HLTDS are structured similarily, however, they contain separate columns with "wide" and "deep" in column names, indicating the survey tier for which calculations were made.
For Roman, we provide results for the following subtypes: IIP; IIL; IIb; IIn; Ia; Ib; Ic; IcBL.
