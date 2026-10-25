Once a clinical trial's database is locked, results are frozen — any edit after the data-lock date is a protocol violation and a fingerprint of tampering. Aurora Health recorded the official lock date for the Veltrexa study right in the studies table. Find the subject whose primary efficacy result (measure = 'primary_efficacy_delta') was modified after the study's data-lock date, and report their subject code.

Use the provided MySQL shell.

Submit the subject code as deadface{subject_code}. Example: deadface{ABCD-0101}.