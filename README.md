# Motus-work

This project uses Motus R book inspired methods to look at local Motus station and tag data.  

Since each project is likely to have different goals and data issues, we start with a file designed to look at project data and metadata for QA/QC called ????_motus_data.Rmd, where ???? is a project designator.  The example files can be customized for any project.  Several are given as examples.

We have split the remaining tasks out into two files:  single receiver with QA/QC (motus_receiver_data.Rmd), and multiple receiver with plots (motus_signal_by_antenna_comparison.Rmd).  The single receiver file can be run line by line to get the receiver databases you need downloaded and to update them.  The multiple receiver file will allow you to see signal strength plots of the same tag on the same timeline, to compare signals across antenna arrays so that we can judge direction of flight.

If you have to download or update either the project or reciever databases, it takes a long time.  Having these tasks seperated out makes it easier to modify just the task you are focussed on.

The receiver and comparative plots are set up so you can knit them to generate a report for sharing.

## Workflow

Generally, you will want to run the project file first.  Then you can run the receiver file once for each reciever of interest.  Then you can decide what you want to combine for the comparative plot, if needed.

A typical use case would be:

1. Notice new interesting detections or need to do some reports about detections for stakeholders.
2. Record project ID, receiver deployment IDs or serial numbers, and time frame
3. Run line-by-line through project file to get an up to date project database file locally and check for problems
4. Run a the receiver script for each receiver ID to update receiver database files locally and check for problems
5. Run the plot comparison file to get some plots to use for flight direction and timing analyses and reports

