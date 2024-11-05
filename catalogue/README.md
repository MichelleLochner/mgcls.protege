## protege_catalogue.csv

This contains the full catalogue of extended sources (i.e. pyBDSF islands with more than three Gaussian components) with Astronomaly: Protege's score and ranking, as well as the scores from author ML. **N.B.** This catalogue should NOT be considered a ground-truth catalogue of anomalous sources as the scoring is completely subjective and assigned by author ML alone, which was used to train Protege and hence produce the final score and ranking. This catalogue should be used as recommendations for interesting sources that may be valuable to follow up.

**Columns**

- `objid` - unique identifier in the form imgX_islY where X refers to one of the original images in the MGCLS data release and Y is the island identifier given by pyBDSF. Note the column `original_image` can be easily used to identify the source image.
- `author_ML_score` - a score on a scale of 1 to 5 given by author ML when running Protege on the full dataset in interactive mode. See the paper for details of how sources are scored. -1 if the source was never scored by a human.
- `protege_score` - the score from Protege after all 400 recommendations have been scored by author ML
- `protege_rank` - the index of the source in the final list of recommendations where 0 is the source with the highest score from Protege and 6160 is the source with the lowest.
- `ra` & `dec` - position of the source in degrees
- `peak_flux` - peak flux of the source in Jy/beam
- `x` & `y` - position of the centre of the source in pixels
- `original_image` - the name of the fits file the source can be found in
- `obj_size_pixels` - the edge of the smallest bounding box that contains the source
- `evaluation_subset_author_ML_score` - the score from author ML from the evaluation subset (where all sources in the subset had a human score). -1 if the source was never scored by a human.