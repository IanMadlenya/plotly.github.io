---
layout: single
title: Plotly API rate limits
permalink: /api-rate-limits/
state: active
meta_description: Details on Plotly API rate limits and throttling.
---

# Plotly API rate limits

Updated August 01, 2017

### Introduction

Plotly throttles the number of requests made to its servers. This keeps server traffic and costs manageable while still providing a useful experience. If you exceed the number of allowed requests for your plan, you will receive a message and have to wait 1 to 24 hours to make additional requests.

The Plotly Web App uses the <a href="https://api.plot.ly/v2/">V2</a> version of the Plotly API. While the popular API libraries (Python, R, MATLAB) use both the <a href="https://plot.ly/rest/">V1</a> and <a href="https://api.plot.ly/v2/">V2</a> versions of the Plotly API.

### Limits on Requests to Plotly Servers

While many functions use the API, The API limits are as follows:

<table>
  <thead>
    <th>API client</th>
    <th>Exceptions</th>
    <th>Per Day</th>
    <th>Per Hour</th>
    <th>API Version</th>
  </thead>
  <tbody>
    <tr>
      <td>Python, Arduino, R, MATLAB</td>
      <td>None</td>
      <td>50</td>
      <td>30</td>
      <td><a href="https://plot.ly/rest/">V1</a></td>
    </tr>
    <tr>
      <td>Plotly Web App (<a href="https://plot.ly/plot">plot.ly</a>)</td>
      <td>GET requests are not limited</td>
      <td>1000</td>
      <td>None</td>
      <td><a href="https://api.plot.ly/v2/">V2</a></td>
    </tr>
  </tbody>
</table>

### Upgrading

To avoid limits in requests to Plotly servers, you have the option to upgrade to a <a href="https://plot.ly/products/cloud/">Professional Plan</a>.
