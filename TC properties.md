First, some definitions:

$$TC_i = \frac{\partial FOM}{\partial w_i}$$

Where $FOM = FOM(MM)$ is the figure of merit of the meta-model $MM$ (correlation) w.r.t. to some ideal metamodel. We note that the meta model is the stake weighted average of all models $M_i$:

$$MM = \sum_{i}^{} w_i M_i $$
with $w_i$ representing the weights (stakes) per model.

Since the figure of merit behaves like a correlation coefficient, we observe:

$$ FOM(MM) = FOM(a MM + c) ,\quad \forall a,c \in \mathbb R_{> 0} \tag{1}$$

In other words, the figure of merit is independent of offsets or changes in scale of the meta model.

All positive TC
----------------

Let's assume a case where everybody has a net-positive contribution to the meta model:

$$TC_i > 0 \forall i$$

Which would mean that adding some $\epsilon_i>0$ to each model's weight would increase the figure of merit:

$$FOM(MM) < FOM(\sum_{i}^{} (w_i M_i + \epsilon_i))$$

But with $\epsilon = \sum_{i}^{} (\epsilon_i)$, this gives $FOM(MM) < FOM(MM + \epsilon)$ and therefore a contradiction with (1). $\square$
