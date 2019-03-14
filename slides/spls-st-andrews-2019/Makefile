EFF ?= eff

all:
	$(EFF) spls-eff-bayes-demo.eff # let's start with one file and work our way from there


eff:
	eff -l spls-eff-bayes-demo.eff

plot:
	rm -f output/plot.eps
	gnuplot plot_example.in
	gnome-open output/plot.eps

prior_regression:
	rm -f output/plot_prior_regression.eps
	gnuplot plot_prior_regression.in
	gnome-open output/plot_prior_regression.eps

silly_regression:
	rm -f output/plot_silly_regression.eps
	gnuplot plot_silly_regression.in
	gnome-open output/plot_silly_regression.eps

importance_regression:
	rm -f output/plot_importance_regression.eps
	gnuplot plot_importance_regression.in
	gnome-open output/plot_importance_regression.eps

smc_regression:
	rm -f output/plot_smc_regression.eps
	gnuplot plot_smc_regression.in
	gnome-open output/plot_smc_regression.eps

clean:
	rm data/*.dat

