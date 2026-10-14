Today I practiced reading and writing to a file. 

Following is the command structure that I followed to make file, read and write to it.

touch notes.txt
echo "Line 1" > notes.txt
echo "Line 2" >> notes.txt
echo "Line 3" | tee -a notes.txt
cat notes.txt
head -n 2 notes.txt
tail -n 2 notes.txt

<img width="573" height="337" alt="Screenshot From 2026-10-14 07-31-34" src="https://github.com/user-attachments/assets/6cc8f8ff-2dbd-4fa8-855d-364eb20408c9" />
