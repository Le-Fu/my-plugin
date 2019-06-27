#### it is a vue npm package for create a simple table


1. table header

> input

`

    test: [
        {
          fields: [
            {
              key: 'k0',
              label: 'h0',
              type: 'text'
            },
            {
              key: 'k1',
              label: 'h1',
              type: 'text'
            },
            {
              label: 'h2',
              children: [
                {
                  key: 'k4',
                  label: 'h4',
                  type: 'text'
                },
                {
                  key: 'k5',
                  label: 'h5',
                  type: 'text'
                }
              ]
            },
            {
              key: 'k3',
              label: 'h3',
              type: 'text'
            },
            {
              label: 'h6',
              children: [
                {
                  label: 'h7',
                  children: [
                    {
                      key: 'k8',
                      label: 'h8',
                      type: 'text'
                    },
                    {
                      key: 'k9',
                      label: 'h9',
                      type: 'text'
                    }
                  ]
                },
                {
                  key: 'k10',
                  label: 'h10',
                  type: 'text'
                }
              ]
            }
          ],
          key: 'total',
          label: '总计'
        }
      ]


> output
2. table body

> input



    body: {
        total: [
          {
            k0: 'v0',
            k1: 'v1',
            '<': [
              {
                '<': [
                  {
                    k4: 'v2',
                    '<': [
                      {
                        k5: 'v3'
                      },
                      {
                        k5: 'v5'
                      }
                    ]
                  },
                  {
                    '<': [
                      {
                        k4: 'v6'
                      },
                      {
                        k4: 'v8'
                      }
                    ],
                    k5: 'v7'
                  }
                ],
                k3: 'v4'
              },
              {
                '<': [
                  {
                    k4: 'v9',
                    k5: 'v10'
                  },
                  {
                    k4: 'v12',
                    k5: 'v13'
                  }
                ],
                k3: 'v11'
              }
            ]
          }
        ]
      }
