import random

class 遊戲機台:
    def __init__(self, 機台名稱, 咬分期機率):
        self.機台名稱 = 機台名稱
        self.咬分期機率 = 咬分期機率
        self.當前狀態 = "正常"

    def 判斷狀態(self):
        if random.random() < self.咬分期機率:
            self.當前狀態 = "咬分期"
        else:
            self.當前狀態 = "正常"
        return self.當前狀態

# 建立遊戲機台
機台1 = 遊戲機台("ATG機台", 0.2)  # 20%機率處於咬分期
