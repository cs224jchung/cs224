cs224
=====

This was a project for cs224 Project 7 polymorphism ALU

==== NEW THING DONE ===

A few days after the project presentation, I was curious to see what could be done to speed implementation of ALU Polymorphism project.

It seems that using an indexer is a great answer to the project.
If I had time, I would do the following: 

Theoretically, the search for the ALU polymorphism can be instantaneous (using an inverted index "KeywordAnalyzer" e.g. Hashmap.get function) by employing Lucene indexing. I would have Lucene index every 30bp letters to be indexed. In addition, assuming there is a 1% error chance, Lucene allows a couple error sensitivity by using: "fuzzy search" for a relatively cheap and quick find.


=====

List of all the classes:

aluGenerator.java // generates a random sequence of nucleotides as an ALU

appendALU.java // File that appends the ALU to random locations

appendEasy.java // My attempt to work on the base easy case of the project.

genomeGenerator.java // generates a random sequence of 3Billion

hashDonor.java // hashTest

Hirschberg.java // Method of finding perfect matches of ALU in a read

homebrew.java // Compression of Genome

KMPplus.java // Slide method for finding matches of ALU in a read

Pager.java // breaks down the full genome into smaller 4MB files

threadALUr.java // Threads the ALU insertion

Legacy:  // contains files that are no longer part of project
	addALU.java // 