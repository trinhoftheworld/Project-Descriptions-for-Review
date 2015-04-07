# Reviewer Instructions for Stage 5

## 1. View student’s web page

The file you receive from students, when unzipped, should contain a file called `app.yaml`

The top of the file should look something like this:

```yaml
application: learn-2-code
version: 1
runtime: python27
api_version: 1
threadsafe: true
```

The value of `application:` is the student’s **appspot ID** (in this case `learn-2-code`)

The **appspot ID** determines the URL for the web page the student should have built. In this case, the URL would be [http://learn-2-code.appspot.com](http://learn-2-code.appspot.com)

You should go to the corresponding URL to see the student’s page.

## 2. Review submission

The student’s web page should have a section that either explains or demonstrates what they’ve learned in the last course of the Nanodegree (where they are encouraged to pursue something that interests them on their own).

I suspect most submissions will meet specifications. This stage is intentionally easy.

## 3. If student passes, generate a “secret key”

If the student has passed, that means they have completed the Nanodegree! This is a big deal. By successfully completing, they’ve also earned the right to add their project to a list of student submissions. But doing this requires that they have a “secret key.”

You should generate a 6-character secret key by calling the `generate_secret_key` function with the student’s **appspot ID**.

You can copy and paste the `generate_secret_key` function into your favorite Python editor.

```python
def generate_secret_key(appspot_id):
    import hashlib

    def is_valid_appspot_id(appspot_id):
        """Helper function to help identify invalid IDs"""
        num_chars = len(appspot_id)
        if num_chars < 6 or num_chars > 30:
            print "appspot ids are between 6 and 30 characters"
            return False
        valid_chars = "abcdefghijklmnopqrstuvwxyz0123456789-"
        for char in appspot_id:
            if char not in valid_chars:
                print "appspot ids do not allow: %s" % char
                return False
        return True

    # Check for valid appspot_id
    if not is_valid_appspot_id(appspot_id):
        print "Invalid appspot ID"
        return None

    # appspot_id looks good. Generate key...
    hashed_id = hashlib.sha224(appspot_id).hexdigest()
    secret_key = hashed_id[0:6] # simplicity > security

    print "Secret key is: %s" % secret_key
    return secret_key
```

## 4. Write Feedback
If the project meets expectations, congratulate the student! They've come a long way.

And don't forget to include the `secret_key` and the submission URL [http://learn-2-code.appspot.com/student_submissions/](http://learn-2-code.appspot.com/student_submissions/) in the review. The first part of your review might look something like this:

```
Congratulations on completing the Nanodegree! You've earned the right to add your project to the list of completed student projects here: http://learn-2-code.appspot.com/student_submissions/

You will need to use the following "secret key" to add your project: abc123
```
