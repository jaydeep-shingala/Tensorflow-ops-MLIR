## The Performance metrices

Here given is the table that shows performance differences between tf-xla, tf-standard, with optimisation pass enabled and without optimisation pass enabled.

| Benchmark        | tf-xla          | tf-standard  |  with optimisation pass  |  without optimisation pass |
| ---------------- |:---------------:| :-----------:| :----------------------: |  :------------------------:|
| cast_conv.py     | 0.1822 | 0.0279  | 0.5437 | 0.5143 |
| cast_transpose_conv.py         |   0.1912   |  0.0387  | 0.5708 | 0.4962 |
| conv_cast.py    |   0.1864    | 0.0312    |  0.5086 |  0.4806 |
| conv_transpose.py    |   0.2138   |  0.0281  | 0.5152 |  0.4804 |
| conv2d.py    |   0.1580   |  0.0259   | 0.5256 | 0.4571 |
| transpose_conv.py    |   0.1878   |  0.0272   |  0.5431 | 0.5271 |

here, with optimisation pass is the normalised (as per instructed) time after we enable the optimisation pass and without optimisation pass is the normalised time after we disable the optimisation pass.