# Deep-learning-challenge-binary-classification

### Optimization attempts
| #Trial | modify | modified (add/remove etc.) code |
|--------|--------|---------|
| 1 | first trial | `hidden_nodes_layer1 = 8`<br>`hidden_nodes_layer2 = 5`<br><br>`nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer1, activation="relu", input_dim = X_train_scaled.shape[1]))`<br>`nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer2, activation="relu"))`<br>`nn.add(tf.keras.layers.Dense(units=1, activation="sigmoid"))` |
| 2 | added neurons in each layer | `hidden_nodes_layer1 =  50`<br>`hidden_nodes_layer2 = 20` |
| 3 | added another hidden layer | `hidden_nodes_layer3 = 10`<br><br>`nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer3, activation="sigmoid"))` |
| 4 | added more neurons to first two layers | `hidden_nodes_layer1 =  80`<br>`hidden_nodes_layer2 = 40 `|
| 5 | removed the third layer<br>hanged the activation of the second layer to "tanh" | `#hidden_nodes_layer3 = 10`<br>`nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer2, activation="tanh"))` |
| 6 | decreased neurons in second layer<br>changed the activation back to "relu" | `hidden_nodes_layer2 = 30`<br>`nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer2, activation="relu"))` |