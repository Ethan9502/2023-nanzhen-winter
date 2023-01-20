# Unit 3 lesson 2

## Step 1

將``||玩家指令||``
重新命名為*parkfountain*，
將迴圈指令中的``||重複執行||``拖出並設為4次，
然後將此重複方塊拖入*parkfountain*的``||玩家指令||``中。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
    	
    }
})


```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
    	
    }
})


```

## Step 2

將迴圈指令中的``||重複執行||``拖出並設為4次，
然後將此重複方塊拖入第一個的``||重複執行||``當中

將代理中的``||Agent破壞||``拖出並設為 下(down)，
然後放入第二個``||重複執行||``當中。

```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
        }
    }
})

```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
        }
    }
})


```

## Step 3
將代理指令中的``||Agent移動||``拖出並設定為 前(foward)，
然後放入第二個``||重複執行||``當中。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
    }
})


```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
    }
})



```
## Step 4
將代理指令中的``||Agent轉動||``拖出並設定為 左(left)，
然後放在第二個``||重複執行||``下面。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
})

```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
})


```
## Step 5
將代理中的``||Agent物品槽||``拖出，
然後放在第一個``||重複執行||``下面。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
})

```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
})


```
## Step 6
複製第一個``||重複執行||``和當中的所有方塊，
將複製的``||Agent破壞||``改為``||Agent放置||``並設為 下(down)
然後放在``||Agent物品槽||``下面。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
})

```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
})


```
## Step 7
測試時間!
將Agent放在起始點，然後按鍵盤的T鍵並在聊天欄中打入指令**parkfountain**，
此時Agent會挖出一個5x5的邊然後將洞口用鵝卵石填補。

## Step 8
將代理指令中的``||Agent移動||``拖出，並將其設定為 左(left)，
再將代理指令中的``||Agent移動||``拖出，並將其設定為 前(foward)，
最後將兩個``||Agent移動||``放在第一個``||重複執行||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
})


```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
})


```
## Step 9
將迴圈指令中的``||重複執行||``拖出並設為3次，
然後再拖出另一個``||重複執行||``並放入，同樣也設為3次，
最後拖入*parkfountain*的``||玩家指令||``中。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
        	
        }
    }
})


```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
        	
        }
    }
})

```
## Step 10
將代理中的``||Agent破壞||``拖出並設為 下(down)，
然後放入設為3次的第二個``||重複執行||``當中。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
        }
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
        }
    }
})



```
## Step 11
將代理指令中的``||Agent移動||``拖出並設定為 前(foward)，
然後在``||Agent破壞||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
    }
})



```
## Step 12
將代理指令中的``||Agent移動||``拖出並設定為 後(back)和距離3，
然後放在第二個3次``||重複執行||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
    }
})



```
## Step 13
將代理指令中的``||Agent移動||``拖出並設定為 左(left)，
然後放在上一個``||Agent移動||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
})



```
## Step 14
將代理指令中的``||Agent移動||``拖出並設定為 前(foward)，
然後放在第一個3次``||重複執行||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 3)
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 3)
})


```
## Step 15
將代理指令中的``||Agent移動||``拖出並設定為 右(right)距離2，
然後放在上一個``||Agent移動||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
})



```
## Step 16
將迴圈指令中的``||重複執行||``拖出並設為5次，
然後放在上一個``||Agent移動||``的下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
    	
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
    	
    }
})



```
## Step 17
拖出代理指令中的``||Agent放置||`` 並設定為 下(down)，
再拖出另一個``||Agent移動||`` 並設定為 上(up)，
最後將兩個指令依序放入5次的``||重複執行||``中。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
        agent.place(DOWN)
        agent.move(UP, 1)
    }
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
        agent.place(DOWN)
        agent.move(UP, 1)
    }
})



```
## Step 18
將代理中的``||Agent物品槽||``拖出並設定為2，
然後將``||Agent放置||``拖出並設定為 下(down)，
最後將兩個指令依序放在5次的``||重複執行||``下方。
```ghost
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
        agent.place(DOWN)
        agent.move(UP, 1)
    }
    agent.setSlot(2)
    agent.place(DOWN)
})



```
```blocks
player.onChat("parkfountain", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.setSlot(1)
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 4; index++) {
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(LEFT_TURN)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 3; index++) {
        for (let index = 0; index < 3; index++) {
            agent.destroy(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.move(BACK, 3)
        agent.move(LEFT, 1)
    }
    agent.move(FORWARD, 1)
    agent.move(RIGHT, 2)
    for (let index = 0; index < 5; index++) {
        agent.place(DOWN)
        agent.move(UP, 1)
    }
    agent.setSlot(2)
    agent.place(DOWN)
})



```


## Step 19
測試時間!
將Agent放在起始點，然後按鍵盤的T鍵並在聊天欄中打入指令**parkfountain**。








