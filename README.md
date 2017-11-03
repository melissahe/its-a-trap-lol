#  its-a-trap-lol

### made by melissa he and richard crichlow (lol)

## How to work with collaborators on the same project

add them as a collaborator in your git repo

### What happens if you are both working on the same file?

if you use "git pull", you will have an error where git refuses to merge two different histories

so you must first do "git fetch"; using "git merge" after will still give you an error
        "git fetch" = grabbing from the internet
        "git merge" = merging the files in your computer with the one grabbed from the internet

you must do something in between to allow the two different histories to be forcefully merged

1. you must add:
        "git merge --allow-unrelated-histories"

2. then put a commit message for why you want to merge the two

3. then edit the file that you want to merge using the vi editior (like "vi <name of file>")

4. delete the ">>> HEAD" part (all of the ">") and the "< <and some words>" part too; combine the changes in the way you want so the file worksall
5. then git add to stage it, and git commit it with a message

6. now you can git push
