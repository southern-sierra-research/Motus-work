# Motus-work

This project is to track how Motus R book inspired work to look at local Motus station and tag data.  

It is currently focused on project #247 Southern Sierra Research Station Kern River Project (formerly Kern River Valley Tri-colored Blackbird Study).

Recent additions have split things out into 3 files:  project level with QA/QC, single receiver with QA/QC, and multiple receiver plots to see signal strength plots of the same tag on the same timeline, to compare signals across antenna arrays so that we can judge direction of flight.

If you have to download or update either the project or reciever databases, it takes a long time.  Having these tasks seperated out makes it easier to modify just the task you are focussed on.

The receiver and comparative plots are set up so you can knit them to generate a report for sharing.

## Workflow

Generally, you will want to run the project file first.  Then you can run the receiver file once for each reciever of interest.  Then you can decide what you want to combine for the comparative plot, if needed.

A typical use case would be:

1. Notice new interesting detections or need to do some reports about detections for stakeholders.
2. Record project ID, receiver deployment IDs, and time frame
3. Run line-by-line through project file to get an up to date project database file locally and check for problems
4. Run a the receiver script for each receiver ID to date receiver database files locally and check for problems
5. Run the plot comparison file to get some plots to use for flight direction and timing analyses and reports

