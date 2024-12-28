# ten-a

import plotly.graph_objects as go

data = [
    {'x': [1, 2, 3, 4, 5], 'y': [6, 7, 2, 4, 5]},
    {'x': [6, 7, 8, 9, 10], 'y': [1, 3, 5, 7, 9]}
]
fig = go.Figure()
for i in range(len(data)):
    fig.add_trace(go.Scatter(x=data[i]['x'], y=data[i]['y'], mode='lines'))
fig.update_layout(title='Time Series', xaxis_title='Time', yaxis_title='Value')
fig.show()
