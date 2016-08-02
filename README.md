# Hanhan_NLP
NLP research and implementation



<b>RESEARCH PAPERS</b>

* <b>Analysis of Collaborative Writing Processes Using Hidden Markov Models and Semantic Heuristics</b>
* It analysis the PROCESS of collaborative writing and predict writing performance
* Inspiration
 * Maybe I can try HMM in my semantic layer, see what kind of key components will lead to what kind of result
 * It's a good idea to record writing behaviour and do analysis, plus time/duration may be better


* <b>Text - Independent Speaker Identification using Hidden Markov Models</b>
* <b>Hidden Markov Models in Text Recognition</b>
* Python HMM
 * http://scikit-learn.sourceforge.net/stable/modules/hmm.html
 * https://github.com/hanhanwu/hmmlearn/blob/master/examples/plot_hmm_stock_analysis.py
* R HMM
 * https://cran.r-project.org/web/packages/HMM/HMM.pdf

* <b> Author Recognition</b>
* Using style markers: https://github.com/hanhanwu/Hanhan_NLP/blob/master/author%20recognition.pdf



<b>Advanced NLP Tools</b>

-- UW NLP TOOLS
* Reverb  (works well on raw text)
 * About Reverb: https://github.com/hanhanwu/reverb
 * My code using reverb for extraction: https://github.com/hanhanwu/Hanhan_NLP/blob/master/reverb_extraction.py
 * Sample data for my code: https://github.com/hanhanwu/Hanhan_NLP/blob/master/reverb_sample_data.txt
 * How to run my code: 1) Download the latest reverb .jar file 2) open your terminal, cd to the folder where you have your text data input and reverb .jar file 3) run this command in your terminal `java -Xmx512m -jar reverb-latest.jar [input file name] > [output file name]` 4) The run my Python code, in the python code, `r_pre` is the file path prefix for data input, `f_path` is the output data path full name

* Olive (works better than Reverb for longer/more complex raw text)
 * About Olive: https://github.com/hanhanwu/ollie
 * Sample text data: https://github.com/hanhanwu/Hanhan_NLP/blob/master/olive_sample_data.txt
 * Olive extracted results: https://github.com/hanhanwu/Hanhan_NLP/blob/master/olive_extracted_output.txt
 * Check Olive Quick Start to run do the extraction, if you want to extract the results into a file, run command line `java -Xmx512m -jar ollie-app-latest.jar olive_sample_data.txt >> extracted_olive_sample_data.txt`, and remember to `cd` to the folder that include both latest Olive .jar and engmalt.linear-1.7.mco
 * Olive really did a good job in my example, in this sample text example, there must be grammer mistake and each sentence is very long. But Olive could find large amount of relational noun. I am also surprised by its N-ary extractions, some of them could extract those parallized phrases accurately. Check my olive_extracted_output.txt, you will find the examples
