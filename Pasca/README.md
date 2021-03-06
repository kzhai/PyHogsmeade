Paşca
==========

Pasca is a naive python implementation of the work by Paşca (2007) on weakly-supervised named entity recognition framework. Feel free to consult the following reference for more details.

Paşca, Marius. "Weakly-supervised discovery of named entities using web search queries." Proceedings of the sixteenth ACM conference on Conference on information and knowledge management (CIKM). ACM, 2007.

Launch and Execute
----------

To prepare the example dataset,

	tar zxvf sample-data.tar.gz

To launch Pasca, run the following command on example dataset,

	bash extract_entity.sh sample-data/query+count.10K sample-data/seed.team sample-data/ranking.team.10K

The entire process takes about 4 mins on my laptop, and you should be able to find the output at `sample-data/ranking.team.10K`.

More data would help significantly, but at a cost of longer running time. For example, if you use the entire data `sample-data/query+count.all`, it would take hours to finish, but the result is significantly improved.

For your reference, the extracted named entities using all data are also attached as

	sample-data/ranking.player.all
	sample-data/ranking.team.all

Have fun!