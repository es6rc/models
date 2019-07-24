### NOTEs
1. in `./tfcode(.py)/nav_utils/get_repr_from_image(fn)`, `resnet_v2.resnet_utils.resnet_arg_scope()` is called with `is_training` input, which is deprecated in `resnet_utils.py`. ([History Record](https://github.com/tensorflow/tensorflow/commit/fa7f79541d1ba1fa6f54ea3474cbf3ce1411bfb4#diff-9635628970d153506deb3602e4e7c565) from github).

2. Downgrade `networkx` to `version==1.11` by `pip install 'networkx<2.0'` for the sake of `(Directed Graph)G.edges_iter` in `src/graph_utils(.py)/convert_to_graph_tool(fn)` 