# My evidence and decision log

Keep this file free of names, IDs, grades and private assessment answers. Use it for practice reasoning only. Duplicate the cycle section as needed.

## Cycle 1
- Released package and version: DATA (Information quality), `NEW-SYNTHETIC-20261105-R2`.
- Earlier packages available: None recorded before this Cycle 1 release.
- My initial prediction and reason: I would prioritise the DATA package because it could help address several unknowns about whether the UAV's observations can answer the flood-response team's road-access question. Collecting images alone does not establish whether a road is safe or passable; the evidence needs to show whether the observations are useful and reliable for that purpose.
- Exact files and test IDs used: `evidence/04_information_quality/README.md` and `evidence/04_information_quality/frame_audit.csv`; the CSV contains F01–F24. These records have been inspected, but individual row comparisons and a final included/excluded set are not yet recorded.
- Relevant test conditions and why they match the mission: The mission concerns road access in a 1.60 km² flood-response area. The audit distinguishes road-segment records (F01–F16) from open-field records (F17–F24), and includes blur flags plus image/reference timestamps. Road-segment records are directly relevant to the road question; open-field records need a separate justification before being used to support a road-specific claim. The supplied times and labels are synthetic teaching data.
- Evidence excluded or qualified, and why: No underlying images are supplied, so visual labels cannot be independently checked. The release says the data are newly authored synthetic labels and times, while the screening-flag pattern is preserved from an earlier lesson. A reference time of 08:30 against a 09:00 image is not a time match and should be qualified or excluded under the chosen screening rule. Keep `indeterminate` separate; do not silently count it as dry. A deliberately synchronized synthetic timestamp does not prove real contemporaneous observation. Any agreement percentage would be label agreement, not independently validated accuracy or proof that a road is passable.
- Analysis or plot used, with units: Primary label-agreement comparison using road-segment records with `blur_flag=no` and `reference_time_matches=yes`: F01, F02, F05, F06, F09, F10, F13, F14 and F16. All 9 image labels match their reference labels, giving 9/9 = 100% label agreement for this selected subset (dimensionless percentage).
- One calculation or observation I checked myself: F01 has `image_label=dry` and `reference_label=dry`, so it is one agreement. The 9-record tally gives 9 agreements divided by 9 eligible comparisons = 100%.
- AI suggestion I accepted or rejected, and my reason:
- Current recommendation:
- What changed my mind, or why it did not change:
- Remaining unknown and most useful next check: Define the road-access question and screening rules first; then list included/excluded IDs and the denominator. The most useful missing evidence would be the underlying images plus location- and time-matched reference observations that can challenge the labels. Consider whether exclusions make the remaining sample unrepresentative.

## Cycle 2
Use the same fields. Explain how the new evidence connects to cycle 1.

## Cycle 3
Use the same fields. Show what passes, fails or remains unknown under the instructor's changed condition. Do not erase an earlier result just because the mission changed.
