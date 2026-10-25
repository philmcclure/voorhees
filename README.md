voorhees 0.1
============

October 25, 2026

Run the install script. It will check if uuid and sqlite3 is installed.  It will also attempt to copy voorhees to the first writable directory it can find in your path.  If the location isn't acceptable, or it fails to find the path, move voorhees to wherever your prefer.

The script doesn't check for markdown but it is required.  There are too many variations to check for but Mark Gruber's original perl version works, as well as any of the commonmark implementations.

Once the script finishes, it will open the config file in your $EDITOR. If your $EDITOR is unset, it falls back to nano.  The config file is heavily commented and should make sense, update the variables before you run voorhees the first time.

When you write a post, the first line will be the title of your post.  Anything that appears after the first line is the content of your post.

You can write your post in a text file and feed that to the script.

You can edit your post by the UUID of the post found in the "id".

If you call the script by itself, it will generate the feed.  If you didn't specify a file location in the config, it will output the feed to STDOUT.  Of course, you can always redirect the output to a file.

All of these tips can be found in the scripts usage by invoking the -h flag, i.e. `voorhees -h`
