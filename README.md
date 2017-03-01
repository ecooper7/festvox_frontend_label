# festvox_frontend_label

This is a minimum example of how to use Festvox (http://festvox.org/) to make labels in .utt format for your data.
You must provide utterances in .wav format, their transcripts in txt.done.data format, your lexicon in Festival lex.scm format, and your phoneset in Festival phoneset.scm format.  You can find examples of these files in the voice directories for existing voices, or read about these formats in the Festival/Festvox documentation.  If you are only using the Festival frontend to create labels that you will use with a different backend, then your phoneset.scm does not have to contain any features (vowel, nasalized, etc), i.e. it can effectively just be a list of phones (in that .scm format).

To use this script: <br>
1) mkdir <i>yourvoicename</i> <br>
2) edit the label script, fill in the global variables with your values <br>
3) cd <i>yourvoicename</i> <br>
4) run the label script <br>

.utt format label files will be under <i>yourvoicename</i>/festival/utt/. 
