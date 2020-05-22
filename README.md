# Setup
This will download Lab 3 locally, allowing you to work on your scripts and upload (push) them back up to GitHub.

1. Clone your lab repository into your ~/ops435/lab3 directory using SSH:
```bash
git clone git@github.com:ops435/lab3-yourgithubusername.git ~/ops435/lab3/
```
2. Copy your backed-up work into your new GitHub-linked directory:
```bash
cp ~/old_ops435/lab3/* ~/ops435/lab3/
```

# Submission
1. Run the checking script. Make sure you identify and correct any and all errors in your scripts:
```bash
cd ~/ops435/lab3/
pwd #confirm that you are in the right directory
python3 ./CheckLab3.py -f -v
```
2. Redirect the checking script output into *laboutput.txt*:
```bash
python3 ./CheckLab3.py -f -v &> ~/ops435/lab3/laboutput.txt
```

3. Commit and push (upload) your lab work:
```bash
git add *
git commit -m "Individual message or note."
git push
```

You can make changes to your scripts and reupload as many times as you like. Make sure you commit+push to do so.

**Note:** Your lab is automatically submitted at the due date and time using the last published code. Any changes you publish after the due date won't be marked or seen by your professor.