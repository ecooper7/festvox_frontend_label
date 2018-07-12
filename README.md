# festvox_frontend_label

This is a minimum example of how to use Festvox (http://festvox.org/) to make labels in .utt format for your data.
You must provide utterances in .wav format, their transcripts in txt.done.data format, your lexicon in Festival lex.scm format, and your phoneset in Festival phoneset.scm format.  You can find examples of these files in the voice directories for existing voices, or read about these formats in the Festival/Festvox documentation.  If you are only using the Festival frontend to create labels that you will use with a different backend, then your phoneset.scm does not have to contain most features (nasalized, etc), i.e. it can effectively just be a list of phones (in that .scm format) -- however, you should make sure that vowels and consonants are properly marked (vc + - ) because when converting to HTS-style labels, it uses this information to populate the "syllable vowel" feature.  Also note that if you are going to be using the .utt output for HTS / Merlin eventually, then you need to avoid numerals as phoneme names (for HTS) and symbols that are used as HTS label-file-format delimiters (for both).  It is easier to do this phone mapping at this stage than further down the pipeline.

To use this script: <br>
1) mkdir <i>yourvoicename</i> <br>
2) edit the label script, fill in the global variables with your values <br>
3) cd <i>yourvoicename</i> <br>
4) run the label script <br>

.utt format label files will be under <i>yourvoicename</i>/festival/utt/. 
