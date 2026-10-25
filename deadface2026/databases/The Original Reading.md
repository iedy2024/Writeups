Aurora Pharmaceuticals ran a Phase III trial for a drug called Veltrexa, and the trial's EDC (electronic data capture) system keeps a full audit trail of every edit in a data_changes table. Most entries are routine source-data corrections — but exactly one rewrote a primary efficacy endpoint, quietly changing the number to make the drug look like it worked. Recover the original value that was overwritten.

Use the provided MySQL shell.

Submit the value exactly as it appears in the audit trail, wrapped in the flag. Example: deadface{1.4}.