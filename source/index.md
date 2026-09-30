# offlineisbetter

~

we're excited to announce the first model by _offlineisbetter_.

__offline-sentiment-small__

what it says on the tin. it's a lightweight model with only 230m parameters, finetuned for sentiment analysis, and with 80 ms tail latency on a ryzen 9 cpu.

[try it now](https://github.com/offlineisbetter/offlineisbetter)

__benchmarks__

all f1 scores are on the sst-2 validation set.

we want to emphasize that these benchmarks are allowing the _same effort to set up the model_, not the _runtime_ or the _quantization format_. bert models were pulled from the hugging face hub, and offline-sentiment-small from the github repository above.

__offline-sentiment-small__ 230m / 80.32 ms p95 / 0.9489 f1

__distilbert-base__ 67m / 66.15 ms p95 / 0.9321 f1

__roberta-base__ 125m / 469.65 ms p95 / 0.9396 f1

__modernbert-base__ 149m / 530.73 ms p95 / 0.9396 f1

notice that, to get the same latency with bert models, you have to go all the way down to 67m parameters. for short sentiment tasks, you get comparable f1 score. just wait until you've got a long customer email with lots of detail. furthermore, offline-sentiment-base (and all of our models) _do not require 4 gb of pytorch dependencies_, unlike hugging face models.

__about offlineisbetter__

we believe that it's time to ditch the cloud. because offline is secure, offline is fast, offline is predictable, offlineisbetter.

[read our manifesto](/about)

come be chronically offline with us. _offline-sentiment-small_ is available now. many more models will be available soon. 

[follow on X](https://x.com/offlinedevs)
[join the waitlist](https://forms.gle/XMo6AQeg7FZ2NAdH6)
