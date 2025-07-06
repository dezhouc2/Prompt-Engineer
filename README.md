# Prompt-Engineering Paper

## How prompt format affects model output accuracy: 
  https://arxiv.org/pdf/2310.11324


## Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
  https://arxiv.org/abs/2201.11903


## Chain-of-Verification Reduces Hallucination in Large Language Models
   https://arxiv.org/pdf/2309.11495
    Step 1: 初始响应生成
    模型直接回答用户问题（可能含幻觉）。
    
    Step 2: 生成验证问题
    基于初始回答，自动设计一组验证性问题（例如：
    初始回答："阿尔伯特·爱因斯坦获得1921年诺贝尔物理学奖"
    验证问题："爱因斯坦因什么工作获奖？获奖年份是否在1900-1950年间？"）。
    
    Step 3: 隔离执行验证
    在独立上下文中逐条回答验证问题（避免初始错误污染），强制模型检索事实依据。
    
    Step 4: 对比并修正答案
    将验证结果与初始回答比对，自动修正矛盾点（如修正年份错误）
