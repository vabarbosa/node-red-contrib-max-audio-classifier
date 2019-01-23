node-red-contrib-max-audio-classifier
=====================

Node-RED node for audio-classifier

An API for serving models

Install
-------

Run the following command in your Node-RED user directory - typically `~/.node-red`

        npm install node-red-contrib-max-audio-classifier

Usage
-----
<html>
<p>This model recognizes a signed 16-bit PCM wav file as an input, generates embeddings, applies PCA transformation/quantization, uses the embeddings as an input to a multi-attention classifier and outputs top 5 class predictions and probabilities as output. The model currently supports 527 classes which are part of the Audioset Ontology.</p>
<h3>Inputs</h3>
<dl class="message-properties">
    <dt>payload <span class="property-type">Buffer</span></dt>
    <dd>Buffer data of 16-bit PCM wav file.</dd>
    </dl>
    <h3>Outputs</h3>
    <dl class="message-properties">
        <dt>payload <span class="property-type">object</span></dt>
        <dd>Prediction.</dd>
    </dl>
    </html>